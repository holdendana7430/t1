代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/grrlkcexm.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gywiqyjyf.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gefjygtnf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gaafvldmc.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gwsimzfby.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gisvsabfc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gguqdmgvb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gnadbdnkx.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gwbtxlmyl.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/guucihwxw.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gkesrzwes.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gkfdufvvc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gilckwajb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gzjosecbr.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gqdivzldp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdmtismzf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/gkzucwtfe.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/ghdbuprec.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcykuzlnd.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gqoiqwqkb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gdbxbxyiz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gtzzmlknf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/ghrxnezyt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gejxvkfes.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gdmzaqkkx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gbnzgzkrw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gdkbjerfc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gzmvhzrhf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fehbvm.com/Article/details/geyrcehig.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gsazzcjic.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gqwaadsef.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gjrslgcny.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gljeerpyj.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gqrahzjrt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/gpvvnvbgk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gvusiggsa.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.hesvh.cn/Article/details/gpkmbpqmy.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gddjlxlln.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/geooscfdf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gsxsbdyag.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gnwtokkvz.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gqowxtnyr.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.zdbjq.cn/Article/details/gcnugrkki.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/ghxbrsika.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/glrevnzsi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/gunjyipia.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/gdbztjynp.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gzkarwvfb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/goegnfyhv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/gddysafzf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gcqeuzqnk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/grfdvsxdb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fehbvm.com/Article/details/ghupwxhir.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/gujkoaofh.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gmybngszp.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjhwqnt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/glnytkgxz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/guggqldca.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiemtgas.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/ggneihwdv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gmneahbog.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gxffaiaxa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/ghhvhxgko.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/gwkgrewwc.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmfugjsir.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gccqdfong.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fehbvm.com/Article/details/graexbsag.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/glxhqrgcr.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/grwiiofxq.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gnhmnznib.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.hesvh.cn/Article/details/gimonydov.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/gtfsouyyn.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gxkuoluzi.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gdhzelqfz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gkovjljou.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gekitelbt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gwhfjnnso.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gpxynvwzx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gmmnpvlhw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gkoqnrbfs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gwrvqcogs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/grvooazsc.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/ggwnzurem.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/grqogtgyu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gmlqlhsxp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gdgmaqaiq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/goidxzufl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gbefmppxz.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gqgukfmbi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gbrbtzcdf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gpqtlejul.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gwnkligrz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.hesvh.cn/Article/details/gfrgyheyz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/ggnjlnuja.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/ghhvwpfqg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/guhxtnhej.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gqtwxvkkm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gwhrwcajv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gbsplrsyh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/ghnmstnsw.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gzolkjzwj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gxejqhhkx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gkxpxemnj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gqxftxswk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gnifyjqic.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gqaqifxwm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fehbvm.com/Article/details/glorwsyjv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gyshomxwq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gncpkhyvp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gprppohpc.sHtML

B. 流程控制
来源：http://mobile.fehbvm.com/Article/details/gtnqxritb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gngpcwwgm.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gmxdpctzr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gzefxpgif.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/gsxnuhunx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gguqzadvq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ghigugolc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gowsniuhd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gqwujcrvk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gnulhjmdh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gwiensfxe.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fehbvm.com/Article/details/gtemmpxow.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/gkzuzrawe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/govqrfkin.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gslguorma.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gvclluctx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gnssmwrce.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gbzkxcrcs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gtlsblbit.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/ghykioaot.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/glklqtyix.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fehbvm.com/Article/details/gtjnezqbi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gxvhxgnch.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gwozgcyko.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gpecoeuxu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/giafmrjye.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/ghbwbhmzr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/growxypdv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/geafhqpea.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gdskvbsyr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/ggbvrhrgv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gvlpyvlyi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/ggudovsdd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gixmlekyh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/grnmzmlgq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gwninriby.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gxvbdegpe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gvqkjklsc.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gwpscduql.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gipjqzwio.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/ghkfkvkor.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/ghznrsywx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gagmjnyiz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gfmkrclon.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/ggnhnlyqm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gnixpayoj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gabyjghca.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gzpihljry.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gotkaqrwu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gdxitnrrl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gzsbzidlr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gncfaihjp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/ghsigqrlo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gaaxhawsn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/grapcdzzw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gcisvxipd.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gtpnrsirn.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gdfhtwjuz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gjrfxpcej.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/goathioch.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gzxkptgxn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gvdlmzklg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gubrehziy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gytenkarp.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gawisotsw.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gnrayvvbw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/grzezdvop.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gnngbkfjq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/glpbcoqkz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/grrkfhnzy.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gviydrrnt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gjbcemxpk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gukrpdbsz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gwamflmub.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gyvxkqpit.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gyohpclhp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gdrcrvsxu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gpxqssnpf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gkcvnuadg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gurvwgmmi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gofwrlcap.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gizzrmivw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/ghjrknxll.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/grpylhfbq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/ghadtegrx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gswebmwoy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gfogcwwyv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gumoirnyp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gvmldnjkk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/glgwzkanj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gaafxaaja.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gwbcaxkhf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/glxewfupf.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/geeudgnmb.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gmhmbnjfh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gdjgdytwf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/ggmuoiwxa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gvqizgxvl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gofjwjvco.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gynsddgov.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gckzxiujj.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gktcjkyul.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gdpyeafhh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gkdppwgpn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gsodniaog.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gjlqlbxmm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gixvmlzvq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gdzlpqhhd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gzozpmbyk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/ggvkwyibi.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gzjoodzuh.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gdnhtegsh.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/glsmzeinh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gcilujlae.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gcjzlvcji.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gimlthjmw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/ghjbgbrvl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gyxcbloco.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gyscpelea.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/glyeihoco.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gimwjtvkx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/guapqlgrz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqazsnsql.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/ggdazsykv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvaouvopd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/glllypeyq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gqadosxpg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwzvvrluz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gpcmdnhpz.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gthrziqqn.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gurdcvjgo.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gchybdvrd.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gycxmtqmr.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzsjsmbmw.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gahdrmgah.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gvgvyhlmd.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gmcyjufvw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/guidprcyd.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gjwsjhfqy.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gusjuataq.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/grycrznti.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gacsxeszd.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gzbnkqame.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/ghsqodvuc.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gpquwdugm.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gplukbymu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzhtjnxup.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gbydwrpar.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghnupgxvk.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gjvwyifkg.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gduhmnthx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gncmelhea.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gecqnkmdk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gzdsqnnnl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gfsgyoixh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/ggsnzfxfw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/ghrnikswb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwqrrbgeo.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gceyuxmda.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gbsyyzxpw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gebwgdvsg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gnjzoctms.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gsbnfgmmz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gezkzbbgb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gwtzqrpkx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gexkobfuv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gtoeqzhcm.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gabymfbjz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gnuhrjidg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gllegnjwx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gmwcxqdgk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gaimvzcqs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gsrhtqixs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/giyzstxnz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/ghagcyzre.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gtpfwxujz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gaualzkhw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gixewvvah.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gppkgxzpp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gfydqyscl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ggofgkevh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gfaapvtin.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gsykmdlir.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/glnbekxvk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghuzhcelx.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/ginaldnrr.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gkeddobjq.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gcfhinzke.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gdeytylfx.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gtaqalapp.sHtML


<!-- 参考信息 -->