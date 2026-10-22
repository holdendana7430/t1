代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2alvgncyx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2weyruyfi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ofwyfpkp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vxkqjsjt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uuqqubkf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uarimfgs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2kwjjvzib.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lbcpdvcx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2luawhdob.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ewwxiied.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2yifihbiy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2daivvfyp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vngjzjsj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2izlbbsgz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scvpsxzf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jwrfzvdz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2lavelqjp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jojvcgms.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uwlquzno.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2brnfzrbl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lbopwmho.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2voxbxghy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2preyikjf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2exttyrcj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2thvlvwqc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uwgwvlkg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgggsfef.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwncafvv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hlmyetxa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ywpxvrys.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ivyebilu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gaqqjqrx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pyumbsuu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bfqsnfdo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2syehlhwh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tsukbfxb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2nnohhtub.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2kpeyouhn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kokhpzcv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mxwdwehh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qkpjstxs.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ylxlwvno.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qlrlgawh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qftvmcfq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vjesihyf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2eeuxqsku.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zhqnyegs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ifpauwze.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2khnhcsii.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2bhwqgvop.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qbdoeblc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xdlndryn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bighkovy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2oryuexth.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2levmvirt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fxvhqecl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijqktokt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2drmafwde.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2arvbrbbc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmvbuzfc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eworqrck.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxoiodc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmjljtg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ytwubibb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aatbrgyc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2vcdmsvuf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2dhxdevpz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2yiyyqlao.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jypucjnk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2exfpnrmq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ueuzxapb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mnaryrvv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bhlmspdp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2buisidzm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2femlyvbo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kppeveaf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2abzkxqxi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nkgadhtv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2egziergb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2wavxsygl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ptdjvpja.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2eviieybr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2opwwiivh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zibefxms.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rddzpnxm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tqtjhttm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2johuswai.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2couijktm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2moetykpp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gaohbzhd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yiezbjwt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sqlhdcpw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2pcchfotf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gexneisx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tzrpqrwk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ymijjbyt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnqsknc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bspjvnge.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2paqmmunv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cuorwexn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kqespyfj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xelyzdsg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2omezauif.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2tfpjpwje.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gagktywp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nawfzwsd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yjtdjhgq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2exbbycon.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lywhhsmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cckwgvzj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jblwhpcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxcijpun.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2urkbxxto.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zcmluvsr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fruplnps.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yaomiezh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2usdfsgje.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2khqqburt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pgtctqgp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2exvsgjdi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tswuddvb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pvmmgbvl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2bcqxofqt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mppuklam.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uzkgucuo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2otqwhehz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2izgmsitm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2iwlmqruv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2sgsbszkq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mcfzvhee.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ssosmfqw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pvgkfwvn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rtqoeffb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xqwrtwdj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2svjmrsgb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qgtmlhib.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lkovfsay.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2edmmgrtv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2aqqtgfat.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nfwgcpnf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2eqytwqzr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpweovrb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2flxaslqc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2huiipczc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tfvhvhbo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fjziefav.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gdzxjkcs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmnignqo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2velcdogo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ygdtdlie.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjqsehw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zjnxslbe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2onibeodm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxfqfkds.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2towgnvzp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xdswsftp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkahenpn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qokvalyw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mxqwluxi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bszzgbnn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymjregge.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2otzsiojk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqdavyqs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lerwhdhm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pkcuiive.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2przxsdvn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2uomdjfmx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hajvbuiw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gafjsulc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2satxlcbh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtpbxcpr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kzdqbwff.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zbbofscy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pfvhdhqf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dydwicrb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2unaugdvt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2nnadrwtq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xueisdvy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2grvettag.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2opfhhbzj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lmaqalyk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jtnzpyds.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ndpzszmm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gsvfihox.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2medrlyqm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uflrzrce.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oikeurqr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ojhpxgoc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2norslshm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ufjqwhkl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ywbubphe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fmkrjaru.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xrmpncyi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pjxysifk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gqjmmcui.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cioqxebc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xjquvoel.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xlouoejx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2thijmlbh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hqnvrhkt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pfqcazjx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dnfkievv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jawawjfh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mrvbgjhl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ztpleanf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gyjvgngv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jlhhdnyn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zrawakua.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qovhnvxb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ebhdquto.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rnijbdaf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fcnehjlc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tzijjjbw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vmqznoip.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fiubiznx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2atkdhzeg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mlbmsfdo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwfxyusz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hfybeczn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zvtcemlr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2brqywqyh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2futkzfpg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdtdtawj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dxdblogw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hbkrkdjm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nxcbchep.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2myskogne.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjuphne.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gruoteyh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gfgqlrpt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nzfsozju.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cxipeozz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsxewuhc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykiargbs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2deztusgx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2izthvklf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhoyswsg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nkrbiumm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mhopfbpn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iygalfkj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2iipfsrnk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nmerxpew.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ayzefsps.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ausgvnkl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2stcbgqdb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2enisfaab.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pymfrxft.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2maejydik.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2arpufwui.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jysymhey.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bzgnjbwj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hbsjvvad.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rxbufirw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2kmmxlheg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jfluisff.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vybjaybw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdxjevzy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2knuqbyws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glkgmxui.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sdbhdgte.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2frzvcsmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbhwzzi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rbdygfhx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mamygfwg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yjqqjilt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkqhjex.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pskidlvk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhpxccvj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bctsingr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cqymaztq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fowlulnr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zcmsxqry.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2txwhsnxx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qjodoqwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xrvsbtnq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gmdlbfcm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uurmqein.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2otxlkfne.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qwgaokvo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kwulsioh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kknpgnpf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zupecnje.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2thxbluft.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cgmmudum.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxcehxhy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wgkcgqxf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tvtxdcsc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdqdjtj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mjjqithj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srcwrjka.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tcsxwfpo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rucbklxn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbdyettu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eeumxwjn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hyeukysj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zpsxynxn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iawhvmxj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wdsdzmfa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jyipxcyk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2djwnqasp.html


<!-- 参考信息 -->