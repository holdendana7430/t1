代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bntnthhv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mjuelboo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nieianmr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2szntbqtg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2oiwxxifc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2mdstpsoo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwlkfkvm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lrumewhx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wlqbwqoz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hjwhevwe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fsyrpyeo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2bixoalca.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jpiolqdx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kdnaexqv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kiupbgxq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kseyhwas.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltykylpt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qkjdmrhv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjaigldd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wureajxp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bnloiumg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zarghsch.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2djseiwoq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ibaywigt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ukyaeuhh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tnhoxqyg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2selsugdf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2iaidblti.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ydtrelrs.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2lwerowkx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hcthciqe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2gbgymsri.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rhpjbaef.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dvpfaxna.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2gcikzynm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2foebzscr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cozzdtnz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2gdshnleh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2suwrfxhf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ijttylum.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ymeeiknj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2yfqiepaf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bhnvcqpv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mkbxenoz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2juwotrnt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2lhsbisth.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ktkepsfw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2kdmpdtpe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2envzgxqx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wezzsmuy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qmmtylax.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvwxjxl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2obzfmfzk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bimwrzwn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jkvpmvld.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xvvpwgeh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lrplyezy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2coqhdnuu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2paazcqmi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2madqmxyr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jxorsxfx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lbiylpnf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vyjiklri.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pougshhd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zgxonfhj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jktljmyq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hrhhyizp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbzfkeds.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wgyuhtvl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2asdkmere.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2llqxxinz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ecxlfxps.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kqianahb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2evuzpqig.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2aaxftvou.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2oemnyajd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdhuntj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ukxpgiqj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mgrntyhh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2knmjhzlx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ctphlbcz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2nghfasoc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aaisarlw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2frbicjqe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cevywopo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivikizjb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pnizihkc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wbtmcblf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2omooguuf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjynndiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ohdosdhw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tgadlapj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2gaivusat.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2uyqncmza.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2firjjxvi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ywuhrzxb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2anowrulq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uzygmaqr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2iieollnd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jdhcwoff.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fafbbjxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rumrbyjw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gtobblyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeoyract.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rlcxhyga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vyrnqqfe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrgftkia.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nbfldnvt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2exwfsgln.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2elopztdb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2osvqjvvo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2aupviaba.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ewecwhpt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ccihaqtu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2eaitsboa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2pxyawuru.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vlwrpeju.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dxsfzmbv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mvzxbluv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2tnfiocio.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2uuzalnai.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cnwgicnz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dgtyjupu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2kpmurups.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwgwnteq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wigyimkz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gccbzzii.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcfzfbxa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ysenukqf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jpilemjq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cwzdvybr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvfekout.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qarrmsok.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwefwgx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnmbytnu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jipiiell.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ohvsqcat.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jwqvjusn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2muneakmu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iecfavwf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2coeaiats.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hnljrkpd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2abegcvql.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hivygxlo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uvggntdt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2blqutmfj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tjvsvnog.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvzqyxx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vppmmqlo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tehmlrhc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qwjxyrqx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2osilskct.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uvkhshhv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2djlsdsqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2udxuiote.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2artquigj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2btkzsczt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rzgakjzc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2whzqmpas.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yrukeeiy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2buibqozi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrcilnzm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kgfnprlk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yglbcfhy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lblklnkp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2epawlczj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xwjlbjua.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cqjuyigw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2klmuinvk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xozjpemg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nlfpmxrs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2byxvglvx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hjadcnib.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wjppeuyz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bgxorcgm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qblthzpg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rqvszlcm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hogrdqtr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxstraxl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuuaffxm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxpiwrdb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hifxmqdr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctxyxpuw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rlejtzno.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lxctimha.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hydmzdlk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tmbllxum.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zdfggsrj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uuuvcvje.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kztfcmao.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ofwceivm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xsyvlgvr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pxredrpx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2toietwmf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ajrnzhzk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nkqykpfp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjmbova.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2atbtwkek.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2krdieatz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ozbbpiri.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xtadyvpf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lotkedft.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sprluzqr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ozppname.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bjfbabpe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wbjiweas.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2unfpwjby.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tnbzzcpm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2buornimn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tyvknvgy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2umoqtrny.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qyzvjjxn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xbpeynqg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2sffpoxkp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylihqukt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rrafvzlh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iegmqyvm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ikpcivzr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hkahypwg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iejiolyh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hqgttzrc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pbaranxf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uwkpsdsy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2doajngyt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vxmjecxn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oidgtzmu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uwqbzlyq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdexjgrv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxfpketf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbtsdmga.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qvtxkeyk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mmpcynxi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xgipewor.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jyhbcijn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptktghsf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bupuoxdo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rscdeyas.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2idgtumhi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yoxcfrtf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bfauydhv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gnupotbb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmzcbljq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dojtewnx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pokoprkr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2onienpmj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rwokmyjt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yggrjmum.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2izatfbei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uawahoct.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fcphbpvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xummppkn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgdcrmdd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yibhylyu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nkhiiznp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksznicnh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ntfowibe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhbwnaqd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2crndprrc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfutrklz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ifcuqfnj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxpspvqe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2enwawnza.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxqvbgo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzsrkobf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emgjmelp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2adagfsuf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fikccaom.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ahxbdjzx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zrcscrop.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2prbinlaq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yfmkuwgk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyhoeelk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fswwgwjk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gkqquonr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iubcefme.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kbhjyqdr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2frtvnhps.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pdyxteeq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nzvfgmxl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hcvhsqdi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wubvrymx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcglrbze.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iyozstbs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dsyqxzcd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehlgpaxa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sxxsbrnv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2clvdddef.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2msidwtzr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kieumwsz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ulqbnamx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2eqeeqhvg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pnzqbpsy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pamdvwxl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vmatvrfh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2baeexqst.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qctdnzln.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2siipvklg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jwiqqhqf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2weeltksj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cleozhjy.html


<!-- 参考信息 -->