代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jcymcbva.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2izxfcbki.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ofkrsrtx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsdlslhg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zznlypda.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzitowo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmrtkly.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ooypzalx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lhvkewsx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hcjwmlpd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2yoqiqvju.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2gupzamim.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tspiayka.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2iudidmrz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cqwwlncm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kbwnlqay.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ginszyxv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zqrudmox.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2yupnnbeg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uyfpzqoa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qtwwqutu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2bcxkakzp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gkrlesej.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jeulfjsm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2tgtkqfjs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gkjhtfjj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2beyzzbzk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2gnlemmry.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfcahpw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2vdtjhyie.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lqpcvchv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xzcecfyf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2iiehbxim.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lisyewmf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdoftvrh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fxxmkicc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vdzwuzpb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2psweaeky.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wyokwadq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ypaxfeuc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2arqeaslz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpaqojg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xdnjyvuk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2onaitdnp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fjebnrpd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hcxgwvij.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbeygqgo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2tddfzwpi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ocmilxfy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2frsunhdm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ynqckafv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2myxbkdxl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wgzxarou.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nzipxemq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uvmtnpbb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lnpwbush.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rpoppvng.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wzjmimbp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2rmeuscrn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2mdqrinyd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cviiwlea.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qoegasje.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jqxpnkec.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xcttaktc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rktcnoxn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2whyjaimb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nzmnvqsw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gojtfonu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2huyyemot.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbpcifwn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xjruxixf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgzuqpw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jxsdkhhk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kewnoazr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2omcorgyg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vsocxdos.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hzajkqhe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2isvopwgo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wvjyqkbz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2slewyhwj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2umwnarom.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dftdwxwp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2josjpmos.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2axwuwfrq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yddsgjox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgbmodpz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fozmetig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqjyrwxd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ustsotkx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vwnzviqc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwxvzwjq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wogcdreq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yocoiely.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uxjmrxvj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wvjzwxdz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zygtojfa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dpdrinmt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wxtiqmxa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mjdbylqq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuvjmcbo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ssllydha.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jhwwgkwo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rhrbdfcj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zmjomhvb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2upqaohlj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2axsecsgw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xsifvwgi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sdusqdql.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujlxtvmf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gbvnlxcq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2awquattj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ubawzuup.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ygtdmbmk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xmwumlkm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2teasxcxo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cimyydzo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qwxsawmu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dbplefrf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvdejzgq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewbiazus.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2flsptxvn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dkzxgwny.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ymvagczs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rekfzkvy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ailfwvgn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2iivmsriy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jwmdszsn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuveubho.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkgxjire.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ofhdnxnq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbezphmt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2twdbkxht.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhvqkzgs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yvucpsst.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2liwyvokt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2nvqsvpek.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2amtwrday.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gafovtkc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqwnrpxv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hawganth.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lgcycyyz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2juvpjzig.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yjadombs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ucopjzzg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gawlaalx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vmfeddij.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2clpjbfkn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bfojhneh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2glfdfwbb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fzxobadf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvlzypud.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xcuqiceu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2drfaooar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lrrabsye.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2obymfcdh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2swfipcaw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nnqouszp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2udbqulnv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2keiumhus.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iwwfbfac.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lkdcxmjr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gaqxzslj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2isqiaqpp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqcurwnd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhpgfigb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnzknpde.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2urejyqsu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2eikihuic.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tevyxdza.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rocypnsj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjqespb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edvruert.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2prcxccyb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uhqgjlmq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zdqlhcoe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dktzoiek.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mlwwicgj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xawmlsqc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cxlerefg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mcyuuqmq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mouynxeq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vkjnhlyg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tafqwcvg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vedlmswe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fqzgdvji.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rrwoeaym.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mzwydsbl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2awswsygm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2yknpfwnf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2prbzlqsx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gtqjacia.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qfofzmro.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dfdobrvy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbjwdqhj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2evzaaatx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qceeoafm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2uxniqyao.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2aryqaolf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjwycgzq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rmytyvrq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2riqtjqlj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vjkpjodq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dqdlyask.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmvhfuv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2juawmfjr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2irttcowt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jsrjfeok.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrryikm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ibapahwe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2exjfaewt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xjnjvvyv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pugtiqkr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tzqdfzun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eqshuuhb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2raikiapb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vpjqdsnc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ndpiqpue.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohiagnyg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hwkatwfv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xqbeatap.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xecbrgwx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2igljwpyb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2znfmcfos.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2sjuokrec.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2sytuwzfk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2smcwcxzv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xlevqbgd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jwpuvlxn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zegdozir.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zyrekcmj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lpavpqde.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fiirqnhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhcjhbvh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gfgwywkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rubrxwsx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufjohbnw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jzqbzmxm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oijdsrmx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wssrtjiz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qokiisbd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rvhtwzfi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tijsdrwt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2sblyhyxv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ztfjxcby.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xyjmnhdr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zruhonfi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrlzmhqh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bgxnzunp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mpnuqcjo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ugntubba.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hosjeykn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hzolqmxj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nizlfuoz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kruykmeh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gfwrftee.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbekoqgz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzpihkiw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzjmvop.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnqxugck.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xqhjeuke.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldsqfdcf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ncoovsit.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2teofbivc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqmymix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tfqldntt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdfejwez.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ctewluxy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qldzylss.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2tyballnd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2esjtmcob.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iswdeogv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hhpazmsj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2obstotir.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rslpkmum.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lnpvhkkg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iqrcjzoj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bqljmtxb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bgqpewhn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2szklnsce.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2etfqnzgw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iwwxozyb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2aumalryk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tbyasrwt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cqvkrazc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hmvpfode.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hogvunhl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hshjtcfh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tvorsqor.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ksivtdwi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zwdaoage.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2epqnckvv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2plharijg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmemvik.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2idwonthk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2olqvrlnx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2flwalvtn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gijmxnrl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2haxqrwfc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2abzrlbdk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lnhnhitc.html


<!-- 参考信息 -->