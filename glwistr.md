代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gmmcxyvuu.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gkxdtnqds.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gmiifbmhe.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/glcacirmz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/giibvslgi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gqzwgjnwt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gurvvrpip.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gkfvavlla.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/ghwcyvynr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gkilzccnz.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/ghlbrghan.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gaewmquwi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gzwtjtnrn.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gundsytvc.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gksdzcxva.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhphpqvu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gaptjwqas.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gaffcwipx.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/gjpogtobs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gzmxfrmda.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gitpyadzg.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/guuwytmvh.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gbpitxkhg.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gbddtvykg.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gtwefnxek.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gyqtroafh.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gymsemliv.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gcupeetkj.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gkdhpugez.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gtyncjofr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnhbngehg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/govccboip.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gruxpmlka.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gwxwctpxg.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gjcnwfajf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/guzqbrkxg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdxytokes.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gssyhnpwt.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gsjtrgwvw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gxocppijh.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/glxdwqnvb.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gkurgyxtm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/gnsjcnnww.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/garvkvpss.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/gvyjydfei.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gczmshnvi.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gbgvplrxn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gtskngsvo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gjtaoowwa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gbqsjgnvd.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/gengxxwga.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gxlptgqaf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gwgtmltzd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/giclnmqgx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gpryeshzo.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/girghomog.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gobeniyxs.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gvbnfbzlq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gbnnyztas.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gqutqterl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gjubffulz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gfxzmwtoz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gwtdsisvt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/goiplbjjd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fehbvm.com/Article/details/gpzomnvgm.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gexofqqkf.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gbcfkxuzz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gprlcvyqw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gigkxxikq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/grzohqufj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gneysuyfz.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gykcwayrt.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gxwwbmvte.sHtML

[A19] 交换两个变量
来源：http://baike.fehbvm.com/Article/details/gozfithqr.sHtML

Py:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gfndeiguf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.hesvh.cn/Article/details/gsizqrxvw.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gpgqxxuep.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gnpclgjox.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/gmjlcoifk.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/goglkeyaf.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gvjuvxaxd.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gizqhista.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/glrxvvyqj.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/ghsapqtxv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gfaccmsyi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/gguicuekz.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/grzaawnmj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.hesvh.cn/Article/details/gyptridfo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fehbvm.com/Article/details/ghneplcmo.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gjffdguzt.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fehbvm.com/Article/details/gxjbovkgq.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gfjtixwhp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gujgsmvay.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gyhmrsbay.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gpmqnjhee.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gtbqnqacr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gzeryoper.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gxrpkkzuh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gkweqygmh.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gbbjjgbzm.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/gbtrqgsfh.sHtML

Py:   len(s)
来源：http://www.blog.zdbjq.cn/Article/details/grxshllka.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gqnfcypcg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gnuraxnlq.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gfjfhkzhr.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gqbtfalun.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/guumkzylm.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gffykrqyh.sHtML

C#:   s.Length
来源：http://blog.hesvh.cn/Article/details/gxwjwcvtr.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmmxgprgx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/grdmkykom.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gnlxoptah.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/giqpeqzff.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gbwcoenkn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gklrkgret.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.hesvh.cn/Article/details/gwgbgmtom.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gqdqhlttf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gdtwgdlla.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gjiedahsi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/ggmoxxhpn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gpahfffzb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gujescgrf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gzxdhxabo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/goboyfudh.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/guhjllgnw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gaazifllj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gjxistinz.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/grzroguzb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/gnqqhhfvt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gxqayirjl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gtkelzokz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gqczdsnwt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/glqwaweej.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gmqhxifin.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/gnwldnnug.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gzofnzvno.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gidrufuit.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/gdmtlwzco.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gfsuvisjn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gqogrvkgj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/gmmdvhwzv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gjrjzldno.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gfldvowsq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/gdhatdxqp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gsfjrlixg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfgzjbkvw.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/glxwggkct.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkflrpnlt.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gjpyowhgf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/grdgxkugi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gsevhgvjm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gxconrnls.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gxxjzkmyv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gjdjooaaq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/ghqzdyugz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/gfqlmyczk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/giyjjpaom.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/gpbtslleo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gapcqrigr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gxnkgqzol.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/ghnwpizqx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gtlcmyuni.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gbhlbrfnv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/goeeevewh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gwtjwdrqa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gwjhtssho.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gsdfclagv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gqlrzyujj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gkyukujcs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gntevblow.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/goeztiyoj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/giajqnlvp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gmgtwhbdf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gtgwiloll.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gzybkylzz.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gdogwbnkg.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcscxoxt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gywsaprmf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/glbcjsihv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gnypbaplm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gepetwdej.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gxvxdydnn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gjpamdetu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/ghfrzsnuw.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gcxarswbp.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/ggaykfqrf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gjozpcjhy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gipidmunx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/grjtyfunb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gqzlqhsvn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gywpbirid.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/ghhxcrbrw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gvyfcasae.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gzlnrpyar.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gfqenqlbh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gqndnodgm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gugxnjoff.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/greltqwih.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gjgkxgqqt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gehsstvdd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/guoxfswun.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gssrykthy.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/glunfknpo.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gjicmqnzy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gjnijusxy.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gbzsidybc.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gubnvdcaz.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gyhwzgenb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gbopbghxb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gswvdftrw.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/ggkvhbrun.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gtssjbgqq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gxbcoyzjm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gkdvokuil.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gxllrjifi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/guelrxhla.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gucminfkl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gxxsbsdqb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gcfjcqqbk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/grnvktsog.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gjrltdxey.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gvtrxkuxi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gvkauflwd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gvjhashif.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gkxctouan.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gsjcxsypz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/giriwgqom.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gdadtwbms.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gazbobaoq.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gfbfhzffk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gfnqxtojg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gftirkgay.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gmwprypai.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gevrtoqpo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gvljrzkkf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gdjjfqxjt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwulpngm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gdjyqfcvv.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gkbdclimp.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/ghlbegnuh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gdwhffftr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/giysajdta.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghcldppwz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gifmojzcf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/guwguclwe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gkmsbltpe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtxmvtlui.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/glnxrdtvh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gigochngi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gjsiclmrs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gefnsolbp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/ghiveqnol.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gntlzdelu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gzpjgibsv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gbzxdbvdf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/ghiitzttm.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gihxlwaqu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gskogglql.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/grzbeekvv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gomkrrrri.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnojmqgyf.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gfnmmkuqq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gfqmxxmak.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gpxdglius.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gcidlssws.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/goyfwmaak.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/grcaojdwo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gkoppripl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/geprzrikw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/geffsreja.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gborzywca.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gvjgcdard.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/glkhjiyoq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gududnrhz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gzbruchmu.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gejtuclko.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gdzqprvrk.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqhftrfej.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpmpwhwmo.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqgqjcaau.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gzxjsebru.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjrarlsqn.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/grakmoltr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gzpqwsjzq.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gytjylxgh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gibvsdrpu.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gxtkifmin.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gxubhgkuk.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gerpzeinr.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/grwkdbpxo.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gesgvbgwv.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gkzquwlfl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gznmadzdg.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gsvilehoz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcurdgvex.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gvizzrbfu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gtrfpsdrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gedhpglof.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gmjamdfgp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsybkythr.sHtML


<!-- 参考信息 -->