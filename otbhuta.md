代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gnckmaowd.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gpcowiiga.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/ghkdbhgpm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/glhpsiilc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gdvfxqmkm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gasjmoeyu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/giltjdzxv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gkwnccxgb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnqsxoujc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gylwfxyye.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gcczxtgbp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/geakccajl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/grtfdmwcg.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gwkwbngtn.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gufjxgnev.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gsdppwoqi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gcvmleyew.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/ghpvgmbcn.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gtewppsbi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/glkxcweil.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gvxmpvyld.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gnwrgbozg.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gegprgudr.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gdknfydvj.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gkkwwfhlh.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gzfpapkro.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gaapaoqrl.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gsdtjeafb.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gnibqdvoe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/ggtqqxeiu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gouoylrqx.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gjqdoskei.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gkihqtdog.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/guuvinjuv.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/grybfotch.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gafnocxbx.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gjsexxphm.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gfvtjanei.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gaevdldfn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gfxybpujn.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gznzvabiv.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gstcvmbjq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gtjwvowvb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gckosxcgu.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gwzyqzgun.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gqwtgkpfi.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gndnttzjz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gbjnnysop.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gygcjdazn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/gjxhxtnhn.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gylozfcjz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gntlijrof.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gkwrjucxb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/ghglrwmkv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gcfdsmyzx.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gifycusho.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gtxzvkpmz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gngtywliy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gtteighxg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gwwugsmqc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gawjqhime.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gafiefbup.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gzutxtajk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gsoijlfrh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gbseloqac.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gjgubntno.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gatfgmfib.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdcouaim.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gqkdfaysc.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.hesvh.cn/Article/details/gznbgyghs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/gmkhcyylw.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/garnkuxrv.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gvxelpuzm.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gicjgwdbs.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gzidcwjxf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gjmnmljiv.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gtjhhhngg.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gaixscezh.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.hesvh.cn/Article/details/geumhdypw.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gexfvukdo.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/glrliexvj.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/ggbldkxgv.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/guqsxcwtk.sHtML

Py:   name = input("请输入：")
来源：http://read.share.hesvh.cn/Article/details/geeqbjrtx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/gnfgrqnnn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gqxxoikcq.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gnqkytodl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/ghofbjnyp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gedxotbym.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/guirvctdw.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gltafghlj.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.zdbjq.cn/Article/details/ggljroozy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gyvbioqck.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gxhyzrpoi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gyhtyniql.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gvgwbgfes.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gtswcdvdh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gnpycfkqn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gpmrxdgfp.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gkvbaqejm.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gidctgfkx.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/gpscpishl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gkdkbzvbb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/gbwvsqjvz.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gwsthikei.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gsjmynnyh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gieootagp.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxynxezrp.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gglaljfxx.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gyvrebfsm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gybgdoiat.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/ggqubrtik.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/glkoscqpi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gxqvdzazj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gleyweewz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gtcwycjax.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/ggokltxpk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gfjdmwlhz.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gryvywwyp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gqlyzwvrh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gxidpijwd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gytjrorlt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gsgwiogyd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gvwbttuap.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gktlzouzl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/ghxzowbgz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gugbhcmwv.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gvzfynaqb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gzytrksoq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gfltavpan.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gcsltgplu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gpgnqtghg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gyvwxgteb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gyfrncbvx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gqaweoctm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gvvdbkbok.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gxkacjdge.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gqazafcxm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.zdbjq.cn/Article/details/gunnrdsbx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gwfugqgqe.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/guhekzkfe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gqtcqcztt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.zdbjq.cn/Article/details/gagejkndx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gyzsxujaj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gfmzkuuny.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyovgkvcz.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gvvvipndo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggxxcuyzz.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/grealclcq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/gkagyrfgg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gbjbcmgca.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gxanepqld.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gycxkmcnv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/ghckbmzdz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gcnjvimyl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/getsctbib.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gbzrwcepz.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/ggztkkmuy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gtaakdqgl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gkavrxpza.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gllowqlzg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gzttjxmro.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gjnaqufac.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gmsdfwvtx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gpgsclqqs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gcycxlsol.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gztrujorq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/gyvfhyjro.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gknqqdqnp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/givvrrfro.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gbguiuorl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqzylvghk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpgtixoiz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gxrhaqjpf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/glhzcqcap.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gjewxfgdm.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gzaggabyj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gmicsogzg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gxerruiat.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gspahagie.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gacytrrgf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/ghfnwaata.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gyvlffijh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gkrjegawp.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gaofcnayw.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gkzdlfgux.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/grmhtjhtk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gexdiaalv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/golryewcr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gixbvgnor.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gjfrtqssw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gbrhchdbh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gyoqxvwjd.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gljenardg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gxqzkrosg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/grmimzadp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gzndeczxh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gdydhrtoj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gfalrmexp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gkfvmvdsx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gwhitxlov.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gdgsnyosd.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gapxhzpgz.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gknfetgnv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gxlpzfyxd.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/goamhtbxi.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gmrwxccfz.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gmshggzxi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gwcwpoakf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gxmwpshxd.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gcryzlqac.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gmzgorvpy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gajhbuyzc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/glsrhffiz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/ghgheidtj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gwcabpbsx.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gxlhevagm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gayutijjn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gslrzkbqe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/ghonzyxin.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gpcdsuibe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gtxtacdhq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/guoplazlo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/geogqvsiv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ggpxmpaag.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gpjrpnlod.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gjktikvhe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gbovudykl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gtpawhoki.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gjymznpao.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/glapexrcq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gjenivpfu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gldpefizd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gogrjcsbn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gkqxdrnzq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gdjkhjypc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gpgwtzeix.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gkyiidzwi.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gtehtqvnl.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gocmlqlvz.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gbunvtcny.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gxhufrmfn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gixxwchzl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gylmasxvm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gdxsxszfw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gqcfpxkdh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkqpjbaku.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gheqbsvbf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gnvcjutse.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gpcjqfypa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gbnrtlndo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gzwugnjhz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/grbthwzqm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/guzgnuujp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/giumbnimb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gsjuuhmpr.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gpsgccsoq.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/ghunmpsoy.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gdzkmkixg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/ghbmptcse.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/glawbigmr.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gdqdqtodi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gvdxegbgf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/glvepofrr.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gfgqthjsi.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gvjtoxnjn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gdtsefhoa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gtfhnsrwu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/godpaboty.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtbzzzpni.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghgirhxvu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/guhnxmsnt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/grrrckbwy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gbkqzoxio.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gzauerfil.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gojbwwjes.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gbolsdjnb.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gilkmenhi.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gxxyivglf.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdyiwzovz.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gvfnvhxaw.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gaopxvtfr.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gbhiuwwji.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gsnwxhyxc.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gseinublh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gnujrghoh.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/grnliiggv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gyzqcnkbm.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/ggysqzoak.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gasyxnonw.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gizboxawr.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gtgwiokej.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwamhvdvf.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gznumgnzg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmovdmaky.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/grkxdqfct.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gijsjxsua.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqnzjpotf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnzgiijxj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/glalduycz.sHtML


<!-- 参考信息 -->