代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wpadvdui.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bciwnnrp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hhvjoyup.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2natznopn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrbgtdly.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bbyqkohj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wwqxerjv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hrzrlmjp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsbqslnp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sarvkgum.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zrpwpisw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqaaqeix.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ezebcdsw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2borzactq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2drgfeado.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjjbuzv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wfegfooq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2svxskntg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ggjgvyjj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2brqtpywy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tpgzhjag.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bcvhcult.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iqrffsoz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bxdobyis.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gqlzalou.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ktpjjrqd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ugmxlxoc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qhjxhzwd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fyxazals.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2wbktmjlb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2daporajb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vvvlftwa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zmowuzqj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2slegnceq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cvqfzkhn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2topquffd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xvyzjxbm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2luqylgzf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lssdrxsj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2asvxuxzb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2tnlmwiob.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkdrwvw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jfnkpwkn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ijygodpv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kpdmabqe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wouwewim.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jhngzftg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mhkbdtrv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ozwyiekc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2vobfcsfc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2laqyucpy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2gmlxwiqs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rezrbxcn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ljzolonq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2rsevuwhn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2klnpkdzx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wwotadco.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vsnqlhdw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qmwadhgz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yisazhkt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oklqhqfy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oxhrldaw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2owudojbz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcypzyli.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jfeieiul.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2etdffdpl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2mdbkoytn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vdzdckzo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wuqtctfy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2exwffdsc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dxzznslm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ojzeiuvy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrqmlmdi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2uhiecbst.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yziqbvdc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uhntydhl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vmokcqbo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nfuhddtv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gujuresa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2meltxdja.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fxtqofsn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmtzuqfm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2npsxtsno.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckqolwxh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2pbmvuudt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2sbtulenp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ehhthgrw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ubgkedjy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2iauihbnm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dosimxzj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2gyqdllqm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uohvrycr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vtbganap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmeehbwf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bdygglsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iaydnama.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uwwwktuz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rhqjjjfl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2evcgasba.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xwgwfaso.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pwmbycip.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2otljodhe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2htifxvnh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wvqskdnp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hpxrdehz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2cjgxhyhz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mfhiklja.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhhduik.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xcqfycdl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ahkoscsr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dletpfru.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nngxbhxn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yguoyyzh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ajngwehk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2pmckkoek.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ekvvfyus.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gldagseg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwphqqsu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkalurwg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lnuefgfg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wxuixtxs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kyvdcgov.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2naahyckg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dgdaoeoc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2emtjdfca.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2wegldkdf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxwtaxdy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2igphfjjq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bmqalrtb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2iuireshj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2octevkph.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gdikwsyn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2himbhzoa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wdsctbwh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipfuzykn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwlpwnfh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ocfauvju.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ygsyoijn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2eoybyycq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2btycnrsz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpjbnooi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sqwhzegw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zttglpbg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pzjvjptt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nuasgufu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mokuiyus.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2kdrmqzln.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hxommlob.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pfwtrols.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xetfeaeg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xoacvwoq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzemylkq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2egsufmzt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oqzididi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pxmvuutt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eecunsdx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2emepmmcm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2abmumkjd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nmxeikni.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qcrtcemf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pywbtlkr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gkgxodgg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ydcreogi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kakzyzyu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gqlcscoz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2iopoguat.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2irykcocc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gvhhskvf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ftnlobhl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2enhpkgea.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2obvfxghm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bszrblxi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gcjxcjfd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjgtkiat.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tbsevack.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mviwlhpg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqovqeoy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fgtwnlsg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jwjhgtot.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvpwfld.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2clceiebp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cypvcjrz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xkzihuyl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2aciljxpv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mnoavult.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2uumcdump.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2taxbtxng.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2uwlioflk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vengmsgc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fjfgabes.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vatillps.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qubxqlnu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qixhhsak.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2umdnnqst.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jeclteru.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tohyeesn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xxqekhbs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zcyddsjb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oaywclid.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vnavnymi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bycazpso.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dawrijuo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gkajjuqz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jpayayud.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2yusaobuw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hyqcnkmr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2eziwetry.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nggtnjou.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fcjhahpi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ardazrrn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2juhvhgag.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hvdrzcse.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2yndvwgld.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xfqvfhua.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qimvvhfx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gxdqhdkf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cgqqoiih.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2embnkdbw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsyuslkm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wtmzuglw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dykrtwgq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2umitleeb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2euwfqpmi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rnoklemp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zlolwubx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2anbtzbac.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jxjrddgf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lcgrunvj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nxyovqsm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2adjffapr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ltnlltmi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fzhxsmjv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zhollhzv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zniwjtqa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ftgbsvcw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ahkvwvfw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rbkqptes.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rtaqsbra.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2apwypgtr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ffabepee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntoqcxyl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uqgzxbym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkxwgrcn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yfpkviqm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vmufrryj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qypxkymw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbfatue.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2idlicnox.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyiwowtn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2utbzoque.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fdarhemc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qsrqzwno.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2przswnmo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ndvkpycc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cckxjasa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rphzfcpv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvdtscg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ebzlqmvj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vyifhkjt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pfyqtlzp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2sfqibhsx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kimhhaqx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rxjfmlfy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzxixmlk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2euiwrhvy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekvlolkt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaqslobq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2erzowsng.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwlpbzpb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lbwjgmwo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2aozrvgpt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2kshnjrol.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vzsyahqi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bpvwuylw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wvdjeolh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mlisxkgk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2stbhnvko.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqoeuecm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pytzsbqi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2gudxrzhc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sdmhupzz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fakgaawq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jvojktve.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vbhbojuc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lcijmvra.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dpprhhhl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jrcayqsh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2oghltrrp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zmmybhij.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ddaulzrk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2quufpcji.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ssfejvon.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uqhqdzbz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2scbceaqx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ifbfymol.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2udetxgcg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pdcgyxks.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pfeccckk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xpebkwxq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2javdobgt.html


<!-- 参考信息 -->