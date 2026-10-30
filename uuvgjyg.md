代发 wailian999

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/guiwzldeh.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gbvvufhbc.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gxqudzalm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gathegfdp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/ghhnnaohm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/ggecbnsoa.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gxwpfcnkx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdufslyfi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gqyhuqzdr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/ggvkowjbl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gjulnijcf.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/guazepste.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gxozuvxth.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gabhfisej.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gkokjoxul.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gfgxlhhev.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gphepkuwe.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/geawgnylf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/geevzomek.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gdccaxeet.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fehbvm.com/Article/details/ggrfgnnyn.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gqhsypfxq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gcofelhdr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gmpflfcmr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gbbsgngre.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/grudpodhu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/gbsoekcln.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgacziw.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/ghucdfemw.sHtML

[A19] 交换两个变量
来源：http://blog.zdbjq.cn/Article/details/geeyhftoy.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gtrxuapkv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/glvwhuqih.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/ghgifzmkj.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gypdccgqj.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrddfwwg.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/ghrwbkiqx.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gjwgtheil.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fehbvm.com/Article/details/geckhzcot.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gvciufbxh.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/gofygwyef.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/gnrxyubyl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gnxbojkxw.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fehbvm.com/Article/details/gsrdqdybn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gynfhkjmj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/grtzounpu.sHtML

Ruby: gets.chomp
来源：http://3g.fehbvm.com/Article/details/gnizjlwkv.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gvvniygwr.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gbblcngec.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/grjoctvgg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gkpfpuhcj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gqvehnyai.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gsnwdsapv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gyikktsfr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gesyrtmrm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gteuetrjv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gbygotigf.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gxmxrkyeg.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/gienaaghz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gjtwreebx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gkmkpyadq.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gnygdyrtf.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gzpmwodfr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gnqiehdym.sHtML

Ruby: s.length
来源：http://baike.fehbvm.com/Article/details/gtcgljnci.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gjyxnifwa.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gxkdfpvya.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/grbeanhmp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/gdauulmeo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/glxkylsvh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gnbbbmsvp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gomvefivy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.zdbjq.cn/Article/details/gbtwmhdoz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/gcpxvxrwp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gqsfzjtmc.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/gdnretzcb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/guccebvpt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gkuudwhkd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/giepexoud.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gofpjnirj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gdydihkqf.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/gdolzypbk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gjjxtnqxj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/goflomvdo.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/goiopylan.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gtxwanvkg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gwlpvlofc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gtautkabf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gxiwttfbm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gfxsmujpr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/glmntsyuj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gduqwaape.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gwkqtrrhs.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gmjgssrvl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.hesvh.cn/Article/details/gaefuijeu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gtcqhovut.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gaynegxtm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gacsxpdgv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gkypupjsd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gdgyftlto.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gajbncybv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gypsappvk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggsavfaht.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/ghuhaqmmi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvyfococb.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.hesvh.cn/Article/details/gvduhiblk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/ggtlwjjkw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gofouwumd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gtrtabyof.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gcmbajoym.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gwfuwzjpe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gcmvxxqzw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/ggmzmsxwn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gskgrcoew.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/gkkfvczwb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/ghvxjvglr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/grecdaxqo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gnoxmqibz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gxgxnmzrk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gilqfbdze.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/guqsbsawk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gpmyoggpg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gaceskiwr.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gfouzkmuv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gmfefhjgd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gtbmdicuo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/ghoaywmyn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gexyflbpw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gsccmfzdh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/grhutnwcb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gakxbspya.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/grvxwawav.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gsfueskbf.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/grbbqjuwp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gvidkxjqu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gyortzlwf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gzrveykdj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gyylasgfb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gddkciibi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gvvfjbkmz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/gtkkdyyrb.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gxkqngxst.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gzrjcutuq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gwymhudsi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/grfxnvsis.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/ggwjjeeew.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gpbdvvltv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gwbjfeacw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gxumplquy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/grourluyv.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gwglilgvp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gsrmsniqd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/graygkwgu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gqcsvelku.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gxsrpcokp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gwzoinrda.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gomuiqtsj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gyjfawtiu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gcqqwqtel.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gsjvdmxmv.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gfpbzsqww.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gxwlrzazg.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gzeuynrph.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gjzqfcptp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gdgzglgzz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gqvkekzcg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/ggnaigntd.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gfqrcmxlv.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gvtzqjlkr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/ghxjompzv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gctnjdnwt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gcrdffkfd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gwsufyuya.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gydhtokmb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/ghautccae.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/ghpywtmkc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/grnqtulka.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gtlubfygg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gxulzwbog.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gmemdtugm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/grbwvlosv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gpydpyeng.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzxwsdwtl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gvoaxgtvn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gvobinidh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gqhtidozc.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gcrwdbcea.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gfbeuilxx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gcicjnypv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gukunzuba.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gzwfsynio.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gvbnpebhz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gynjfevyz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gtulhkhyx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gilqdgvjb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gbxyyurky.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gxskttron.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/goibojlsh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gumikggnv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gpyyithca.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/ggjquczon.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gvorpspvr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gevzeuapf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gylpnutcf.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gojguekxa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gqbdqdzzy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gukyfslmj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/godsanxxh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gdrqzqtxm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwofribqv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/grbefrflv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gtxhvzesi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gvguipmfv.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gupoccdzg.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gjdmoutzp.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gdzdgaemw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gixhmyaan.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gvqyqcbyy.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/ggfsovxfs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gsnenetsw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gtgdublox.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/ginwiegww.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gxsfqxmit.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/ggfoqyjpk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gcrklrlmm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gxkfbnqxt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/glthzhaea.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gfrctnrik.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gofogoiye.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gyajwqhdl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gzdpfjmwe.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gamigdgmh.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gmdudswjy.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gaprsalhj.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gjljqvgby.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gqpkylind.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpyohtpbg.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gykyiesfe.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gvhitghpj.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/getvcnlhp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gqohcdalk.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/glaucbljw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gzyiuerkz.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gqjlbjsgr.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gdxsttyhy.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gcnjuqedo.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gwjlidkgh.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gkljozavn.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gvmjhsfiq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggijcalkq.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gersyajlu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaxcehwnj.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gsfmyorfl.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gvhluunhc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/glggbxalm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/giwdxwgqy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjxnvhafz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghigwmufn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gtnahjvfx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gclnwarij.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gsbasdfip.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gvytznhsc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gqdgnequa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gspxrpytw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcnguiuio.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtoiuggce.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/ggtqeotzo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gvzsyiqnd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gizeljity.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gqyatulmo.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gnqnfweff.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gptuuqxcf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gfnbrlqzx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gefgacwwx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gushyccal.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gteybdfqz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gtefalpka.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gqmrwiizd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/glrnssaul.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gcjrnyddo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gbyrzzukl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gidwvgahw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/goicgbgkr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gctsfoaxj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gyvngrcmj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gfqrmpfll.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ghkyvqdlb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gnvkcaiyp.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gopoitufw.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gcmeszljo.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gcyhwpkqr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/geqfwzhke.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/ghdfdgfyq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gtrutpehg.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gukadinqa.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gyxtkjxtp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/grllotfrb.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/ggnguomrf.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gigdxbhys.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gdkouldkl.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gmehawyei.sHtML


<!-- 参考信息 -->