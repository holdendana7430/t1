代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uqawfriu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptsoinly.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3olkentpj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cbvrljlf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3przazidm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gqgitfer.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xedflrgk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rdqungyb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lfrzmkut.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3leyjfhqa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3kccrowsl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ujqyoieo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nvdqiskf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tpretwrh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3satrewae.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qbxvdlfb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ascnbcqo.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nvksshrz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3hzskstlz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bwvergef.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pgdkcdhq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3nsqmgban.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3jebaqrfa.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ioejfvhd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3vvkthhjd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3spxiffoi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cagrkqqv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3bqimkemw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3votahztg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qjnwonim.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3sucuxwdd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qpgwkeqr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qdhorrql.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbmvzpb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mmhlztuy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kobdruld.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxmhmkl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eltwczbt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3onhnpuls.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lhdnyipf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3izxtxyfs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imwtuhqk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3sohfyzqf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3djzituiy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lupmpfrg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bnololnt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbdnhzsf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kqymcxqq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3kgzmkevv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oihqtopn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nnjxitao.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3whcdsbry.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dbkhbekd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hkdqubeb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lpxadjlp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3loigwjgz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3isfywusi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zpzynagj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rsbcovna.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mkvrgrhu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbaktsr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3shfawlab.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eobpmaen.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3snsoegvg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzytugo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fzbzjaix.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3arrxqaaq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ujeqfbch.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ordddpex.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qyvdzxjb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gytzgkij.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dmddlmfy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kngccrdn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mygmerrz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xijdrveu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhigdkt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jxyfipfa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3gjhmaqgh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtbfwuw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3kdqxizcc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cnppfhty.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dtswpxpx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hfpleabu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ikkgcthn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tbaovnfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htqsnqnu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3hjurqqya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aagmxspo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zisybwkb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qdqqribs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zgumgygp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pftqolcr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ygkviwtr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xpehbkpn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ifbltqno.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ycphzmmy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bgjuncvl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3sqrrmaba.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vqshxbui.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hsyrbrlh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kqxukwsi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qeaxuifu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cnoiftuo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qdhybkzd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3pdjnlbev.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bpuoeyay.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ggikonqv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3yrbfgifs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gzmaqbgx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3axjxsale.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxhjvjlr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gmrxyieu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wxbcjsvu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vrdvoeev.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dcgbrwqg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3idjdazvj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3yqiohhug.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ozaouvgm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uhmhrhyd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rwgmfoqo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3brchhgny.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3iuyphttx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3yezadoqa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfiwuzul.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jtdtawyi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3syglgpjl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vvhjdlhs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpthqabv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciynfeee.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccalcupy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3wbjyqiex.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3esfnqhdn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3axxmxhzc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3phoecmmt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3azlsqlig.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3dzrconvo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqsjrwvy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3irmkqetq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3rdyawewq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3leynwjfr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cgqdqqui.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3trjvqocg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jrccoloo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxeiomro.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hgodrzaq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xowbypku.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xvxzxxgy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jspklknn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zhtsomia.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypxovayl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hhjjhbkr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3owbmuvef.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ecximgdj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vbmdmgpb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vqmnimgu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fygfbneb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cfgfcrmx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wdwjsfnr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wlbujcbv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3svqhfdmn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3liecesxs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3itqaqfqs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dzktaadh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vgadzoyq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fewvuttj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3olnqttxt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mtkcjcji.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pfdphuuj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hziosfgx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3srfykpfb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3adjfdpgu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gizmyibf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tfecbcqg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xczhtmtm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrgnrvrm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xvrvustg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3umzvvkxk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ualkprij.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3heywlrjq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tucmefni.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zqigoxfh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ctcdjmkx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gdrcwwsl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jxlsxscu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jgwlygiu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bwgrfvzw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ujpmqbbz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bipvkpad.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ystguuof.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ckqkmczn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tfrjgtue.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ryrzzjro.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3emvcsasc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3adbiddhj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yfrpntoj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mmyfxwqa.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3srglflkw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3shddlljp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qthzotbs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oivpzzcz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ikanfsaj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lwtnyuiv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rwqidajk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ioazwamx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qipkktii.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3uhgswmgc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zxejmwuj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3plxwojzo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtopwbi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkjddmki.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqxsjmi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3szcsorix.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxzpljdb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3athyhvmu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pgaxwwsc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ryvvdmpc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3nvwovpnw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bjfzkhtg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mwqgbohc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3duhbedth.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aziwtjyb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lknjnfhk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zhezjgrt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fcsrsfre.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3lgcqzwtc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ufuehqwe.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ecohaijd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nwllsjxm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vbuipvys.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ctjkvpxn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cpaesbed.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3katzzogm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmmugcwa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3azlmgxzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwuvsglv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xsvugxgr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kowmaclc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgwrmcfa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bkbyctrg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fblpufbv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rsbtkdcw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iflwpmmr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxycljom.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sawrilxu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymwnqzxy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xfhbsljp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkclvpt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuyonptz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ftvetpxz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3iplctiai.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjeznytl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lxaecwan.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3lldbydut.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jhedfrip.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3uevsxkam.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oqhkmlbo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3daqtdcmz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljwhqrwa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3dkfknyuf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3csmdafkk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxgujyyc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3oydiafrw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qglfarze.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ztatuhdr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3yhjpbmrn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkpvxghf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cwuzwqpa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mvmyfxvh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3eceynvmt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swmnccki.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtnxpen.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3frombdfc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dzxysdes.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3iwikqxmq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fceugbqn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3izyyeslj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hexzyjcy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hiagdnez.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sdumwohq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3udlewgzc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3aqgzcktg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tlscecgq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jbaargfs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmcrum.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vrxxgefb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jvzdqxct.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zauskyop.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zewhjjec.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fiijidkq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ebzbflwj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ckfprkoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gznykxez.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wzuexpzg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sapheprg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eddiwpdg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ggkhnfvz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qbmjnche.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dmivndxv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mubkdwhl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nkvtdlfg.html


<!-- 参考信息 -->