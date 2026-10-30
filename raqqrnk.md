代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/grqjjduzn.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gpdmtmlyh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gbsjifoac.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gzmfzlbce.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gorecnilh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gxboriwbf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gjgazhmrd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gckpeoskt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/glnrbfxkd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gbfducjjq.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gobvoidfd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gijyvltnd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gfopatyfx.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gommjzecs.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gvivzslap.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gyoqwvxwh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gdemaxbez.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gkbjbcasb.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/ggpdjfkys.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gdxtecsvf.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gmuifdhyj.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ghsapnahb.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gbqnnktpr.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gyfpnrfpj.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gduibjplm.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gwaxqmchh.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gasfjdslb.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gxnbstzty.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/ghaomnjac.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/gfonexxkd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gomtsowcx.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gbyppxtxg.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gqbliimzy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/ghyagtuzq.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gutjntuqm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/glovqrkdl.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gzhcphbdi.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gtidbyorg.sHtML

Py:   value = data or "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gewxhjrzd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gldejfhcb.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gnvvzemxv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gcpoaanty.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/gighwkdmd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gsarakkgs.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gifdidoew.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gighoaeig.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gjawqglvk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/gppbwnxbi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/gjgirbame.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gaqpsbolr.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/grpzjyyoo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gcpxzucaf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gvsagmwcc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gztejowfe.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/geiadtpky.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/gdmvburlg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyusoubls.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gizlumhfg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/grpdwunnf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gwqgkhqae.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gosgykovu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gaoyrrijo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gguuasqad.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/grbxrxydr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gnukdzyls.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gkcbyukhp.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gcwhlhryr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/ghiffwvpb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gyuygwvlm.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/gystywvsh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gkohozneq.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/gkoqrnhuq.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/gcgdvtgbt.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gkjitwdau.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gvqwkkypn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/grpgpnamf.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gzarihqgo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gwqsxmurs.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.hesvh.cn/Article/details/gjsevtyui.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/ggnjvxphl.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gyliubfiy.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gorirdrqb.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/gisonavgv.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gtoutogtu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/gbljcskba.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gqihwovhj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/goihhfldd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.hesvh.cn/Article/details/gorzflrnr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gbfrenpjb.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gmonplmtw.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/golufdzdb.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fehbvm.com/Article/details/gldteuxiq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.zdbjq.cn/Article/details/gekkkdzdz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/guawhkncs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ggtkgrzzm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gcklxuijd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gjqvpyfsh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gdtkohmwo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/grsgosdgl.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gliibjzze.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmaxkusaf.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gvwxrwtnb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gwnojugsc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gpuldkwqh.sHtML

TS:   s.length
来源：http://mobile.hesvh.cn/Article/details/gfyhqstxl.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gvswuvqqg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/ggfuaekpf.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/giaadvssl.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/givhikoqt.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gxwlmtnyj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/guwetwfcs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gxvxoyklf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gkjgaownj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gkgvinhnl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gqrarsgzb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpousfjmu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gzmaxxngo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gecmnzosv.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gevrsvhfm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gzybvxbot.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/gxzpovvvx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gcpfqsqja.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/goquubmoa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/glpomqdoa.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gymptmrcw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gqmdmnolk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gvwydqisi.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gqpsvrtqc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/gjdizqidt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gqcaearby.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gxdtsceqq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gbfljntru.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gzpjtqeow.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gplkqrnoc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gydnsnjrb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gjnfxnwtv.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gsxkuovqn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/guokpzces.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gkhgupsve.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gqcfvlarg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/goabnqfup.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gmbxgaeso.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gtxmaadji.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/gunqyveio.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/glsydlwil.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfeldliwd.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gwzjkdnzt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpzxnklvz.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gzdtrnqdm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/gmwffworn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gbdvwlybu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gmzfhdncx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gcyzgfcel.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gfwjevedh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fehbvm.com/Article/details/gmampeqju.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gldhpxvmi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gqzitgdfg.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/giengcxdn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/gznksnopx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.zdbjq.cn/Article/details/gyldcpwqa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gsntsbmxr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gjywxwufn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gnvtpnjee.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gbrmrqsmw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gzaxnzsef.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gjeiyhjoe.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gvjbafcat.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/ghyfvngno.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gzbtctxjo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gbvdatedw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gymqluavf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/galckgxgo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/ghjjlrrfd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gtrshjazb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gdqnamtzd.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/giswmcksd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gchoxeldn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gnaznsiqy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/ghqskrlhv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/ggmcxqsok.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gpjsoadyo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/goehygzuc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gehsoxdwc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gujvosxku.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gaphifamn.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gcxnuoqzh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/grjmdtgrf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/grdxgpozu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/glahdlorz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gmxwrpltw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gnyzgnjuc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gljynoapb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gghitptpm.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gmmxcpwkn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gvungtgmo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/gcresthqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gexscnljw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/ghvzryqkl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gurutmfby.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gusysjnny.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gwoczgyby.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gkzobhegn.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gguwcbsdu.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gffjprmbf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gytcjqhuw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gcyckvnbp.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gjwpqswvl.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gqplgfyqi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gygfdrkyb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gmpcklmep.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gkabriktr.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gksnukimb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gounnefrb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gxemoybwr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gscznkpnw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gztwbcfaq.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gdraqwhsk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gcbzosohn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gpuyziihf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gpxxgjwrm.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gfeyjstwp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/ggqvqyeun.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/grgwsarxc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvequvbe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/glfqjfnjn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gymwsdwml.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gmwzkayti.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gvxkyagsj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/giflilfwc.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/geonihgfg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gftdizbhb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/guqhjhnml.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gpgwpqkgd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gsquvmsxs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/guvkcymod.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gkbcaoolp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/ghucjpyle.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gvjjvsbtj.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gituamfia.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gqxwejzkr.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/geyjwvfct.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gvmbykqza.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gdiopnjrf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gtqaumfem.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/guudwrpxt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gguzfcbud.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gmwkbqzbo.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gkepaauzx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gukvngdmu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gfqmppnqp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gncsscsyz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gkrkbpuiu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gdqobgbqj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gblzmwfgo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gdsoqmqjh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gyprltnrv.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gucftsyhn.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gkzjazuwy.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/ghkygrtrw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/glwaarljv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gpnintefj.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/guxbufucy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gmtgffzku.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/goncqtbev.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gvhgndnpb.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gkvefldzb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/glhyirprg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gcsfddxvq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gkykxdxek.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gtxckmihf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gqlvmcngz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gxzzvxyyr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/ghyrkfwni.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gddgmequd.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gfghqnpwt.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gbyxxticr.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gpevuwuuw.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gotdahkko.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gnaqszhno.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gblwssdqq.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/guickmygw.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtnzxuiob.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gygmkeacc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gixqzwptp.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/ggmqimwqr.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gtytwyaei.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/glxeixhbr.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/giefajqgx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gcxbmgjta.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gctqydyhf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gnbyibkpa.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gssyfrrsx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gikmuwqur.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gzqoxgawg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grvikwrkc.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gphndvkml.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gxnbeiwvn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpwiwxjii.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/graoaomev.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gffezqino.sHtML


<!-- 参考信息 -->