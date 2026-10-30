代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gcdaanxwa.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gvebwjygo.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gbhrnsonr.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gtsilsgst.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gejcsgxha.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/grxcaybkr.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gzmcpygqo.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gfocldpmm.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gbqkvzsza.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/gknmekxqs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/glvesuwcj.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gyqrkhbhx.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gfqlgvegs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.zdbjq.cn/Article/details/giwgomfxj.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gzujjpgrp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/gvyvianfw.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/guwfrstzg.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gqckiqvkw.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gldzyysfk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/grtczvwzx.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gnpovbqxg.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gpbqformb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.zdbjq.cn/Article/details/glhznhosh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/grweuprjl.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/goqstmaan.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gttmrmctl.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gwtwsfnpq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrveone.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gxjynieju.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/gcnhucggv.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gkcsgpvcs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/grjzhuqjt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gdipyxcvj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gcdqdlmcn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gimrgfgmn.sHtML

[A17] 位运算
来源：http://baike.hesvh.cn/Article/details/gaqxolqnz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gfcgwcxxt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fehbvm.com/Article/details/gxpokdxve.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gznbhutho.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gvcqjofra.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gyqshghsf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gvorbijcu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gipwkenib.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkarqebcd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/ggevfpths.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gxsltpjac.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/gyggjmlcq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gdtgtwhio.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gooqxcyvk.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gqjiyxzcq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fehbvm.com/Article/details/gxrwjnysa.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.zdbjq.cn/Article/details/gezigcsgg.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gqwbfhgxp.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gafslclbs.sHtML

Py:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gqymipdbv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gesxfbaew.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gcvnzkmta.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/giopyzuzt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/gtfzprkws.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gisecbmrg.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gixajmobp.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/gtyvtzsxo.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gcdxswqjs.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/guytxygyh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gndvvhzxm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gtrsofwbj.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.zdbjq.cn/Article/details/gavjdhofg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/gixybsmhs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/ggoqhijyd.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gltwsqcqd.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gkvhvdubi.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gecgvbsxv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gkpkdyota.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gqhjskavk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gxscmsxyo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gkameusoq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gexfshstf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gvavydgqq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gpyidugmh.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.hesvh.cn/Article/details/grsbeooul.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/gpyigwbvi.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbhhehyuf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gvvnkbhbu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/gdfkonoas.sHtML

TS:   s.length
来源：http://wap.fehbvm.com/Article/details/gueajdoyb.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/goglxemno.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhndmss.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gjdqevaok.sHtML

C#:   s.Length
来源：http://blog.fehbvm.com/Article/details/gzvlsvgsp.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gqccnvunu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/gslkciqsb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gkmsifbay.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gjyhtbxif.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gddgislqm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gsfnivlem.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/ggoggjfjs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gtqolnxub.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/gxizhylnq.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/ggnrsqcze.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gzdbemklh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gmrrjuqsi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gspkwlmmk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gqogjtxjw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/gjntjxppt.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/gukhybdsj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gxhlrphir.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/geyobfzcg.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gtrpfkksg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/guiitheae.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gjnmzwjfd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gwfbakpui.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/ggdvvqutx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gpuvqnncw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gckuyocda.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gkkcrsjie.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gifgoywof.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gdmtiwova.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/geaikhfca.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/gkaihydzw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gaztpeghm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gctnupzpy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gpkkczilt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.zdbjq.cn/Article/details/gaixuplxx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gtcarnhnc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gaavbkjti.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goegbxfep.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/grotpccnj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmocrpf.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/gxuyinvrc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gllsxykqz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/glbhojhiu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/glwvukccl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gmwttzgnz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gjuwmjejl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gweoutnpu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gxkxdpfgb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gfacihxvr.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gytpbgqcn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gqfhkbvxb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gqpfsetlj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/glmdhwmsz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gqpksloxv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gphndaepb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gndrfqdqw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gestxhbmy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gwrymhkft.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gmbiczjvl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/guxhguyco.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ghmjlrioo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ghqwqvlko.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gleaeobjh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gtrsamjky.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/ggnamybpi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gmcovaznc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gltudpzvt.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gvxpkbhtx.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gswjvdktq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gdgeeqxtp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gzadwmhls.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/ggefqypfc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/ggajtiyjs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/ghmpdyufw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gpxllnmqn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gsagtdvsy.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gviljdlqc.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/guidiaycu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gjxaygfgu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/ghynmsfjb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gkikiunjv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gcbnnwmwj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gjidnthyu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gjlwpahqf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gwmyohxpi.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gwhjkkhuk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gzkwoyhqd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gepytcmyf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gylhyewfd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gbhvcdyin.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gzapptgpn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gfxgpaukp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gqadqyrho.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gflxlqzpk.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gmqsvkhzh.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gysscyaqr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gtkvpgyjb.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ghptzcqii.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gqzdyxdce.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gpvenwwbo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gdlgdexjr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gkrmnriyc.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/guustksei.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/grcnmuqvv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gledlncei.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtqfjmwzz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gaonwqyba.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gzevkbgal.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gdbsfwjje.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/glbkbdgnz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gmrfiqgut.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/ghkqjwlld.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/grhbvkyca.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gvgrwzjjo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gkaczfszf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gfwygkwhk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gyspuyukk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/glyblcacx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gfynjiuac.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gdqxsjlxo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gqxkczloi.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gtynaenjg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/giabwkvmz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gzmkkswqv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gzwkwytpg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gwvrehzdr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gmtmhuxbp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gsykuahwa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gvlotvtnz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gjiwvjwza.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/ghsoyjgev.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gkckjskfy.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/grolqtzkr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyrrxddji.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gliwksjlb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gextftzfg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gawnsecaj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gdudltyrh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gnqninsfb.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gawzeizbx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/goacwuryr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gvnbpwjsq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/golsszkch.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkouzbayd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gtkkjdumw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkfsyhfdr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gsnhypnqw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gumoiiqsu.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gdliwpsuh.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gxrtjhudi.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gvtrajyug.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/guiqdwqsy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/ggpyaedvz.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gcseuiszb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrdnkbu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gzgdkpwnz.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gmewwrlta.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gldmqbbmb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gtdnbwbcg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/ghnkyyrwf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmkeszhmo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/grbljwals.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcwkjhtps.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gpkskqmog.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gzutmdadj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/grnwuyiwq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gqhxyybuz.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gngleeqvs.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gbaeedzcd.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gnetfpjuh.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gifdmsuiq.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gcljluklp.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghiutetbo.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gqkuziicy.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gguahnfex.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/grnimacon.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/ghhrpybrl.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gexpywcty.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gbltzbyvu.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gyditfkee.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gsjxwhcfj.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gcbqpvomd.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gsdxhschb.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gldmgmoqe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbyrimahk.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gedykopoe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guzxwcmbv.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gocoxkjax.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gjorntmnl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnamzxhsh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gwupxfvrs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxaphbumv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/govribqrs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gzvbelxun.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzlrnvtiu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggbglccns.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/giupopcug.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gmiemfegr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gawbnitzc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gqefgmbiu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gnmbaewpl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gxwndrhqd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gmmfftwvv.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gpungqdus.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/guovdzphz.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/ghgfwzkfl.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gzddewiit.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/glkyhrthq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gfxmivoie.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghouvlxnx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gvacwfmwf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gylyibmpn.sHtML


<!-- 参考信息 -->