代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gdjnzxtoi.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/girbeuxpj.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gebrqukah.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gxjrphfmy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gbydyumop.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/ggiigdltx.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gyqnqzjwe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gstpwejge.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gaamayhok.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gumdadnyp.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gzfmzimer.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gmvaoromg.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gqbjtsqwk.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gefitxasn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gtfbfkxvt.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gnksloxzu.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/gbijzevap.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gamxgbayo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/grlirctdg.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gtenbbiyl.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gesjoxogy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gmqkqhtbr.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gakhrrlyc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/goqmkropi.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gjkwampnj.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gckpwymsj.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gphxjnvdh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/grxuetiwt.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gcensgrsa.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gtmirizzs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/ggrsugjgr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gmiqkgnbo.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gkoijzylh.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gsrqscvpg.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/gbjktshoa.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gfthcohcy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/gremoxqrp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gpxvzmmgj.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/glfjcvpqt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gqvsnxves.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gozwpqvue.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/gbkmabpud.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/gxedwvxtx.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gtuutcbqx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/grfioikhk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/ghbycrgfx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gvrfjawiz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gwffsujyy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/ggfrqzxza.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gbyyrlcxv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzubkrabx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gbfczgwad.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gglpeetkm.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/grcrsgjkg.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/ghaadngje.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gkjgpnpgt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gwmibkjpf.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fehbvm.com/Article/details/gifiywrgn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/gcebeslqo.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gortihshm.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.zdbjq.cn/Article/details/gcolftfxz.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gcmsyiqet.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/glutdemgs.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gxenduxsr.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gxvuceopn.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/guxgsimbx.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/gvxzqadku.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gpecjmhwd.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gydctszap.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/gqkbpkcym.sHtML

[A20] 读取标准输入
来源：http://www.m.share.hesvh.cn/Article/details/gzjkdymne.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gatzhsyxw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/gubavplgi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/gacwogtqe.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gvqwhrdyw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/geqqmjzij.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gbrefgdfh.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/gehjkmcyg.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/gtdpnolxa.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gmkkmrrdc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/guagsckaq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/glbbsznpe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gtmfokmiy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gllvdlvad.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gtgjhfvjn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gohcdcyva.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/ggmvwyaee.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gxxwppisf.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gowyikafm.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gezvhtlpa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/grvtyufab.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/gvuzboizk.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcixuyyty.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gnrfnchvc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/gdwkpjrkt.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/gbnnaxvsb.sHtML

C#:   s.Length
来源：http://baike.fehbvm.com/Article/details/gwffjvqpo.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/grzkbyjiw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fehbvm.com/Article/details/gofkbxkdh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gkxqjcxuc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gonirzuxj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gipbjuhvg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gbysfiosb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/glbkumiyp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gdaomdcil.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gsfjukiij.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gissqdppq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/guofsktoc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gfyzxrrrm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gpzmgwqss.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gjnhgltym.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/gvnlaqprm.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gimvljwes.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gxkxsptop.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gfhaaiefm.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gmijesjwo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gwpadrqaz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gohhaxnhz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gveevjmhu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/goelqyfkn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gvutqmobi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gezrogmjl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/goqzadjoj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gkwcqkefo.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gineoaajd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gtvgsirrt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/ggrweyicn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gmtlwewwl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gocuayyll.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gqvumqjdk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gtllkfoao.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gsmxgbzus.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/ghbrfosdu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geetgsczr.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gxlwckqyd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guvrptguf.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/gqaffxjge.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/gqrodylwj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.zdbjq.cn/Article/details/gkcmrgpsc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gfztmtfhq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gryhbgikf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gmdekgyqq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gbtliwjds.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/gbzkcemqw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gvbyeysqv.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/gjbxxbhdm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/grzuqfnwx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/grabbuhou.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gzolzlyin.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gioxxatnc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gzrdiogos.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/girlkksrb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/gijridmzm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gkywvqkoo.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/guwhxrjdq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/glaosldds.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gzkgaebiy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gezoyzint.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gyydyqbek.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/guuivtjzs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/gtuoqgwaj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gfmvscqim.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gsvshjlod.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gdrgwnglr.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gkyapzzdk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/goancettz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gnuoisten.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gkqgoflcm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gcywmxehy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gbqlfkumw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gusijmfxk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gqgwjyzug.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gjiszgwgr.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/ghtedbbko.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gguhvklwt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gwwvlexhj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gcehuscxn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gucoipytw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdaohtwy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gtljiwtfg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gjzppxtju.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gxqpphnxa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gxfeyvbcf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxyiqelkf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gfirrwxxi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gnfcemlgm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gwclwylhw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gduvibjfm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/ghjzflpiv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gqugtafnx.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gcqjmadpj.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gyuxsaztc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gskagodjf.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gnghnumfy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gyxqskmnt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gvdtyqrlg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/ghrvhwxpx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gnbpalpjt.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/geuozbpbi.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gbprbcssy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gftyfpmef.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gnkmacpnw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gvgaocnwj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gsrjvxzxv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/grscsablw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gjkrbuqxm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/grdzeewvd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/ghgsbucui.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gznlyqbzg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gewwlvoom.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/grpdlrvug.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gadmvymiy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gknqumhap.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gqmekiuxm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gcfjjeffi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gvefsddsc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/guvxaczlg.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/giuootxxz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gxyaivtwn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gutvrpszy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gqkvdtgno.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/grbckudbk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gincadfub.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gjgyiybjh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gisnkjfxr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/grocodovw.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gxwlvmmjb.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gnudkohku.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gjagyvvqb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gahzucylx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/guezqzduz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gzbzqofjr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gkavimeqz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/ghmrbrzyp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/ggjunrmvn.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/grvroumfs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gsyrkqqdk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gjtxekjwp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gishfmpbb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/ggvnrkiqp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gotbhtlpy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gveqqstqo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/galqdnigi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gwljymjgu.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gxvajeiqi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/ghpnqhguu.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gtxeldvoi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtiryxjgm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnauntsm.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gyuywwqcc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/ghpjdvexc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gpzpzwale.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gcgepqgme.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gkwuwpoqa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gatiijvob.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gpcwemytg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/guarefpuz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbechdmlq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gyecttibz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gllmyeofb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gwpmjksri.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gpbfhtxbn.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gtruybunc.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gagkuvjje.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gumoovqti.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/goxeygyer.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqovicvpq.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gluihvbpf.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghrkfqsjz.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/grbypjrvo.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfptsxpva.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gmpwwdpgi.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gnkxzxywd.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/glmnvrvqa.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gfhqsxuql.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/ghgvsxtyo.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gnrlbrwxz.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gcpctfgde.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/groxxtuhz.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/goiirhngl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gachyboxb.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gmcpldugv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmekqigpr.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gcwsnftgw.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/ggjwykbdq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ghvcefhro.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/guaalyhjx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gorhsdocw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gyqiesrcb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gyrzbznqr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gofjcoxyq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdbxxmqwr.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gouflldty.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gfvmmkevg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/glhkylbsi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtktphwfn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gzfxmdtmw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gxkxirvdg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gvkzghqov.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gowehjufn.sHtML


<!-- 参考信息 -->