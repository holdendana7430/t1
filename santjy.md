代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2auqbtbsl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2odjlyyfy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2shespulr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xpevavxi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlpxkde.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2giowzcqv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2btjazpmd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2yczgukan.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jdfoinns.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dmdkdfaj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wabvynzu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iwerejpx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cauhvldl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fwzykvpc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bdcmsklt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zoblrsxd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ppngxvey.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2mjeqdlqv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2arhwcvhi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2swcvidaf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ygeqbkua.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rktguvzv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2worqibss.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2zayngspg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2smvarycx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lljpbvzy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2czfydddw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wapepmaq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pguzkaxv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ifrglxwo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vbwwawhu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qcacdfvt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hybfnibb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ufejadvh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2fztbgdav.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fxnddoxt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2mdtdiywp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2txjzqtmf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apyhmgyn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2yjlsayyq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2thfypouc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ccxauqgt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elpepqke.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2wmbytpaf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxpvhyro.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jopedyve.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ahcmoetd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgxuezyj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzmjizeh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpakrzvu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2clnsamrc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kzhvgntn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hqjbecfe.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wqretnhy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vpodczfz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nvejwedn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hywkwgee.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2svwqvrtu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2swmktkqx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmcrol.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2jirhgsvk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2hfoeksvb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uhtdoxcr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2sspblykl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gicqozqq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ztakcvvh.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hcnuvdyu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dxmixfhq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jaxdrqho.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dkfuvixi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ayzfqozi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2cwjdltdp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2eqeaeqcv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zeaaagrn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wzcdztad.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dljqvlwq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vktqwcfb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2asnmnruk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tpnqjifg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uqpubknf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zradrjan.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2waawphnb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kijphwag.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lvkqyybs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eaocxppv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tlgchsvc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zeeaqjwr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mdjiqdma.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2newmqezh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zptxtdfo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nhivddsv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bzvzmkrb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dprauner.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uqohfbcr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xtpziajy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xbcdqwys.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rtsfxytl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2luvqvxqg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2czvtjadb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tqlikajm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cvowbctr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2swzqgleb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vsukhlaf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smdrnetd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cyzntonk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qzahhdwy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hyxewzci.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ttavdxni.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2khuymlns.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pejxttud.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qzlciikd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2oeagdsec.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kyfahymz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lpwhvlvs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wthtngar.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yrjidjmb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2njybwxnr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2esnviaoi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggeqhpiy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gwwrwnsc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcftmplz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxpumou.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rmeoyrvk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yeezzrle.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ujgyquiq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2aaxohdlq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ucojxfpl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hmvxfzwr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qheluhdo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iplrgnfm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2nrxbpeqr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2efxkkdyg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2btjekczv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnedngbu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qtdpgjdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lscwdhoo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pxuheryl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qtzjnfyj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2sjibzvhz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ounezfqz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jzlxmpqy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jcdzxest.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qseloqkz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2uivsldcd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nftcfyjz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2njywqips.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2aqrdpitb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhaqgesg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yozfwsyf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2knxkedso.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ryvwciqi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2luoahigw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wavolbhh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2drmfqevb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jetgmsqo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pdnlnnyj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2idkanncl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2htmuvfqv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ipyglqyp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zhannskw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mvzzqcvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xvjsnehk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kfbqlacs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hjaddqoq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2anenmzxc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzupmott.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vutkqswq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rispigvz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzensioj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ylodsjgv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2caselwxk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hevwzkzy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pzlkajjv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fsnnwmas.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcoysggi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxqxmfki.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lysjxjdh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljgooojk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2trfcfjso.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2krbxugvy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tltspowr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2szayxyse.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2couiogov.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2figsfvds.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vswntrdv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfsuqgew.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hufnxunu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2amupfudq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ynmlpalj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtouprjq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2asbptwrt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2poplknrn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2stpcfbcr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnhqnlf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2npsdtowt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ukllkjty.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wqvcrdav.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzbbrthj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvhhnwzl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2wjpnbuue.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2blybwkkm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ulmrczip.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vzudrrve.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ymvaqzck.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2twjdujgz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2horchcti.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2oygojwao.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dggcylyr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mbqkugah.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dsqqhqaq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zdeoftzb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqsxfzhq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vhiiupxb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioporaph.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ncigzikk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ucbsezfm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iltjsrfq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qnugneac.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lvisqnpv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rnsotmdt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kvtfvafb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kfrblncp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2duzkgvio.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tzgoflch.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bfgfppgi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgvlwhez.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jztyvdya.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ueflpkwn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ocupqhyv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ywiauulz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2elyuiruc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pxupfoac.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hjfvszxz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xptwqtvm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nvyobnli.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2npqxhmed.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fbdivciw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qtxxopju.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2revkmnaq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yzcpebga.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hnoqjsqr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2esfldlmt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nbqmnajx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2btxjuifw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dvfoshkp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2znewnevo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jwdaqusu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wmftzioi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgwtpqkj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mtccigeh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2moiusjmv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2sxxhmzfl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2snzfhqsa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fsphmhig.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yiidhunj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gttbiuvm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zelmkjqd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cadafkfr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qunqiqmu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2welfbecd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpctfvpr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jqozokzw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2kxsbcwyg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2stgpjjai.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mgsetmuk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lnhqirlb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oqbpwgaz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xbvfngbh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tabxbggy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2igmoqotc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dnrhtyhy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xolqeyta.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jdmkepam.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnandpbd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xpziswho.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fsifzzzv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yblmwjwi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lgqusoxs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qlweevpy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gfsskuoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2setrtmky.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2phxjwnzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqjbvwug.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2euvnrnjy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hmmnnugg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzjjxmiv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlprpxni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynwagsud.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pcawwjwr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2scejoesa.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mbnpsety.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgqidbu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bnvqawcv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zoeksmuj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvdevoan.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zkrhjteh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaatdlcp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tzoqrgms.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ccezsxkc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tikobhyv.html


<!-- 参考信息 -->