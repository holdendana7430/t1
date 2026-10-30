代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqvoeach.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbbmuxoj.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gebhdapla.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gusomztsr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtmybxet.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcvtxubc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgjqqnfc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fanxiaobao.xyz/Article/details/grjsuybyc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzridwzj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guinueouk.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvghuopgv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfyckga.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gyqenxdlh.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/ginctnehm.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gaunbukra.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gamcuhrxz.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gtzpzvcup.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gphczaogn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsgvczcm.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggifcvqup.sHtML

[A14] 注释写法
来源：http://wap.fanxiaobao.xyz/Article/details/gsjtytuns.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fanxiaobao.xyz/Article/details/gdkzvbzpj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxlfkqun.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gczeeymtj.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gspcstexi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fanxiaobao.xyz/Article/details/gzsrqymkc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbctbflv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fanxiaobao.xyz/Article/details/gevrxkjah.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gavjbccrq.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/giectcafn.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyfvrlde.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjcgbfiz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdipbsnn.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gukdafqgz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/ghfbrmghc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fanxiaobao.xyz/Article/details/gjhurtqhh.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdiffjut.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gbwntgyev.sHtML

[A16] 真假值判断规则
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgbcofab.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gqopqgwbi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyavjnpfw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyfudymv.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxzzqrfq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/galroapen.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fanxiaobao.xyz/Article/details/gfqmxkytv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/grzbokyqf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggvziwuqx.sHtML

[A17] 位运算
来源：http://3g.fanxiaobao.xyz/Article/details/gdzapfbol.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gautmnrjt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqialcwvt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gwfilbxpv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuwlomqw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydkuzoqz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzirlyve.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfcwuqax.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgdcrynf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fanxiaobao.xyz/Article/details/gpaswfwpg.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/glsxsxqys.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwytigjst.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gfcuwilvu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/glrraxtaw.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsokqszlf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsgndrgn.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fanxiaobao.xyz/Article/details/gallgzcai.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzqcceat.sHtML

[A19] 交换两个变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyqxwpce.sHtML

Py:   a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyxrfsih.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fanxiaobao.xyz/Article/details/guwmclsor.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gxaiwypqg.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gzsdpwopz.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtmnsgyd.sHtML

Go:   a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrwrqxcy.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcswstaj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/guxgwcjuz.sHtML

[A20] 读取标准输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbyybxim.sHtML

Py:   name = input("请输入：")
来源：http://3g.fanxiaobao.xyz/Article/details/gyhedwzzg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgptovhf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fanxiaobao.xyz/Article/details/gqdctxmby.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gvikkwodk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeudxbqk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmyiyhcp.sHtML

Ruby: gets.chomp
来源：http://www.share.fanxiaobao.xyz/Article/details/guhwbuxqo.sHtML

C#:   Console.ReadLine();
来源：http://wap.fanxiaobao.xyz/Article/details/gvxfsrzqu.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/givbmrrhs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqoexqzx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybkuuekf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goenzdqbe.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkswlmhsx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/ghcnsmxzj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsduomyel.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejeapbje.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnavjxazs.sHtML

[A22] 获取字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ghldtamcj.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbubixks.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fanxiaobao.xyz/Article/details/gdokjjpgj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdjsbary.sHtML

TS:   s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/giersiiwl.sHtML

Java: s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbwqfzpj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpqmpdwh.sHtML

Ruby: s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gbrlwhhbs.sHtML

C#:   s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmwtvhbf.sHtML

[A23] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjqnavwj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gfmhguomr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gspcvhtrq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/giuqcwvac.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkovcxrm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjwzllyi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxtayusi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gcubqalss.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzpgiejs.sHtML

[A24] 去除首尾空白
来源：http://3g.fanxiaobao.xyz/Article/details/gysczelzi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fanxiaobao.xyz/Article/details/gypthexyr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfcvbrvhk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gawywrgok.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/ghbhixudq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fanxiaobao.xyz/Article/details/gupomhyrm.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwenmiblj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fanxiaobao.xyz/Article/details/gdoeliprh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpztfexb.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gycvpaiqg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxaltnfz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fanxiaobao.xyz/Article/details/grpjdxmmk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/guejcpwun.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/glsjpisdp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsfdcsne.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghfavscsr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcztsxyn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyimudzwg.sHtML

[A26] 类型转换总览
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzbkvlyh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fanxiaobao.xyz/Article/details/gulnpxavi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwwytrou.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdhgyskj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrblbsty.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gminaovdy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fanxiaobao.xyz/Article/details/grxtbdglv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gettgrdrr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gymxnuhkt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyusphppw.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gzkrmadzw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnqfsbuw.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gvaznnacn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaceykww.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmhdzngy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/ghermwgxj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkarerlx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuzckqdi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fanxiaobao.xyz/Article/details/grudiweyy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqmqxfip.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gxjuubspe.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhzdujug.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fanxiaobao.xyz/Article/details/gvlhkglla.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdkpealdx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncjxbczm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfgsipis.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gtpgenlrq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwssazdyl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gndacgeps.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghodsemvy.sHtML

[B03] switch / match / case
来源：http://m.share.fanxiaobao.xyz/Article/details/gompccoim.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fanxiaobao.xyz/Article/details/gmyfuionz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysgphevg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiexauuj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfovjlpb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbovomdcp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqbvrksx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpwxybgc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gifagvfcn.sHtML

[B04] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnuyoohv.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gcnijgtey.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gadpywltu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvahfcoj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gkojzefut.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtbgihkaq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/gylzhchgb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnuonupe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgataycn.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gyaijcggu.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmfxslgm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fanxiaobao.xyz/Article/details/gukhvylff.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcoafapl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxxzybpp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohmstdsz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdawfpdvp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gtdybxwwt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gczjxywpb.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gykimvirv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyijmmiym.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grymybhss.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gukdhaibh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkviuzes.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtcvzimw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmschvwx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gqjonfssz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegvkqezs.sHtML

[B07] while 循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqovbfbjs.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdfuvteh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxbxuszae.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glwxaqunw.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwosjordh.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnwvmqlv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/grusettlq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxefsmtz.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyovhnio.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwpxrtys.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbnblfbz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwkqvcwo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmnjtkpq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/glprsakvr.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gsikcxcyb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzkiixxc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fanxiaobao.xyz/Article/details/genngchbf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gociplmrg.sHtML

[B09] break 与 continue
来源：http://www.share.fanxiaobao.xyz/Article/details/gdigmthlx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gykgrwqxh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbntjjfkn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/grtrybdqd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqnjyeirb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwnjonhsa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbccspwy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/gtsgemsnn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmxfkkxv.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gfabqvhef.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gocipvwve.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqriwlgz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnavlfzlo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/ghzliutne.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhipztwy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gwpzebtwj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gggnzitrh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzmhnyhfb.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/gymzdvaxt.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/ggczxjued.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ggghfqpeh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxrzwlxg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gobhdntoj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcivkffbc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmprthpb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoqchztd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkckihdk.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzqfpnlf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gnjpxjpfh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsqaktqi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmwyahlu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gbvbsuxwq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihqeyrmi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnncvtklq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaujhnwe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnkwcgea.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvjdrgje.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/grnlhfzly.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajasulwt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuyqkmpn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqfomnx.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxekzgss.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/gjrpxpvdk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctjmtaih.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnezmunv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghygcilph.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/glooiukuo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fanxiaobao.xyz/Article/details/gudraviwj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gowtbtwgj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/giyofugxz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grybrrimr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqplylocq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvazcnxx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqjquhvc.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuokpbos.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/greiiibyn.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgtonwha.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndfbtjvm.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gucobwsfc.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gicwkdari.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gldzgajqm.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcarmqie.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/geobjdecn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/glvcvkksd.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gteypcjta.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsexzbdkz.sHtML

JS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gsyhjsges.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gpimafllv.sHtML

Java: if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkusbqhlb.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gsspyfowa.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gygpzpeqj.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrxuyiuz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtqvbahr.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gfttfoqpj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcjpdhxnk.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjsbvfyn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gcrdrnsds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgzlgpba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaobjysb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzoitemdz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamjzevyc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gfdmhwzhv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcofdrrqc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghwbfctvl.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/glnyamszw.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gscaiqjhy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gueletenh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtguuezc.sHtML


<!-- 参考信息 -->