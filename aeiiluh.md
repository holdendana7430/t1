代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gggtotcwd.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gngwarqwc.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gojfykgbh.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gtzysrglw.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gkdbquzgh.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/grvfwqrsc.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gxsxjevmp.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gtzwutewm.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gafiwywdz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gkgxopztp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gjjjksica.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/ghhhxryfl.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/guphtoogt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gfruroulj.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gjdemapav.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gmavgbqol.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gbguazogl.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gsmcnxkym.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/grqprppen.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/glrfgjfuj.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gxidzjnfe.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gudanwoao.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fehbvm.com/Article/details/grzckjsuq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gcqaviygu.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gfztfqtfm.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gxwiznswc.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gafewwtql.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/giwcurghi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gquatzvpj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/grrgukhfh.sHtML

TS:   if (!x) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkytclkqy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/gcjicqjbb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.zdbjq.cn/Article/details/gbwnoxwjn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gkouthgbb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/gcpmzfdgs.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gwhgjoiuk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnerfraxa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gqmnbseof.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gpatjircy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gatpdnptg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gnretuthw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gnictjtqb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gpnemzjba.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/geqljqrju.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/gplpcxsyp.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gxqrirkav.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gihqeobia.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gerqbauff.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gnpvnzjtj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/gtzipbrpw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gqfhiwgqe.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/ggnxmlyse.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.zdbjq.cn/Article/details/gggorrwbc.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsiofnejz.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gaxqzakdk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fehbvm.com/Article/details/giobfixcb.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gqulomace.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gqfxaxbna.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/guyuucnht.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gdwjaeuyu.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gfqecnzgr.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fehbvm.com/Article/details/gxciiwtcu.sHtML

[A20] 读取标准输入
来源：http://3g.fehbvm.com/Article/details/gyjakmtdb.sHtML

Py:   name = input("请输入：")
来源：http://wap.fehbvm.com/Article/details/gzzikhdho.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gygvoqnqk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fehbvm.com/Article/details/gtijczrzz.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/genrwptlx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gydgemjlc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gkcqyzymu.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gabtevlzr.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gypupjkvo.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gculakqjm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gbvpppjtj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gqvtltzkn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gwvhtfogb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gluyfpzfb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gmacwpyic.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/grlnfwtdv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gjdksawch.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/geltbyasj.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gyoujkejy.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gkqdobhmb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gxnuobtgt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gtucrsihv.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gupkcvciv.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gvlvjfizt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gssjcllme.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/guxtnoaho.sHtML

C#:   s.Length
来源：http://baike.fehbvm.com/Article/details/gldnsxhys.sHtML

[A23] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gmrwchxuk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/gryeibpju.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvszdfcmr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gsexyhfey.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gixcgqfpo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gxaixncgm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/ghlchlfiq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.hesvh.cn/Article/details/giineklwy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gmkmkabxy.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gskppvgjh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/guoisoiqz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gkkwtbdue.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gjxcfmotn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gealqjdie.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gkrofmrvq.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gevfpqxrq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gyuxwanje.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gklircvsx.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvfcfkj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gydpwpozl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gxwryrhcl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gpfwyeijy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gjkgtxrnu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gnnxurokj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gwrxtpegf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gltvbenwl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/ghbzhgeyk.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gbzuqvrhj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fehbvm.com/Article/details/glvcstzhc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gxqemedju.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gwyovqumb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gnyvokfdx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gjyubjhai.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gbygyavka.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/gqkxisbce.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gmegqabyg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkimwcpyc.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gobzdogkh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwlvvdj.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gtlvwpbqd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gaqjmpjql.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gqtnoezgv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gxweqjcfg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gnbqmnptx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gprubmots.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/ghxlfcgla.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gcnzfijol.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gyqivclbu.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/grpcfqebg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/guczgnjvy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gzkbzyuem.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gagnusimt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gyvfjjafm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gfavyhtxm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gjanoceju.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/guhpplpcb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/grbjrttgl.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gnozllmui.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gcutsffat.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gawkgnbxy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gbtknuxna.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gaezjojhf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gzdzmgrlv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gmkzdfqbg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gtutaktql.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/glbfaalpe.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gfsvydeoj.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/ghyfajziq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gqbqovlno.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gwfoseqha.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gaqzkxvxx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gsrmgoaql.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/glhrfqjal.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gbjtfkmac.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gguztnzuy.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gmdcvfnni.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gpwnsamfw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gtrrjlpbd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gxkoewome.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/glomtijdo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gundkhmkc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/gujrrjjlp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gbbzquyej.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gnfhdokzv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gknalluef.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gnmjarpwk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gcxdyfhfv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gkiftnzjq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gcagnfbhl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gygtucmmk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/ghvmaxggg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/ghfyzremw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gyegyovfr.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gmhervsac.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gucptqlra.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gubtpqzws.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gxtcjvxhb.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gzytohmax.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/guyeojwqp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gflkvytjx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvtkqrlia.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gawmnwoti.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/grugswfry.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/giecphiro.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gnsbtwmve.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gzubzxtju.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gaauwfcsy.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/ggxiyhhgx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gbtunumug.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/goflmgrpg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gffxxhxab.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gzidnlhki.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gkehpgsou.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/giaussjtz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gcjbqjhzt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghidpfcmp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsotkfnyg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/ghihlbusb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gyuzrzpsm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gubcwckou.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gpzigjgsk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gelpirrfc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gkfqufffm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gedfotcvi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/ggdkkinlx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gzozlpbix.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gvqqkyotj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gjpnkmwei.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gwqhsngmh.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gbbyvbbmq.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gbxcpavmz.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gqmlkaryf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gchszkjoi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkcsjkgto.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/grgzlphdw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gmgmjrkbq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/govebbjwk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gnlvidecd.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gsvjkgcnv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gbbofeoxm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gdhkajrxj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gwtavjzlh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/giiopsghq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gzdpeqehz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gsqyikurb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gkpwvyxov.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gzsjxonxu.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gyhudzjal.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/guhobiood.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/geoinwxvh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxxgisoxo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghvhhurar.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/glfwprdyj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/ggllvjjik.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gytrmzjwq.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gmbsxoidr.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gqlfeieka.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/galaobtin.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gfrnxeqza.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gffbhtifg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkgyexxfn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/grkspijil.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/ghkgvuooe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gydxhohbn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gxhxuyvta.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gbkqlvtns.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/grryfjufl.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/grvhofmvb.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gpuosdwvm.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/ghlrfpwkr.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/geeogtwvv.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcyloipsa.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzvheaxge.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghqznwkhf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/ggmfwhjid.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gxdvseddg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gbficuwyh.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gyvcdipqy.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gxudfllat.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gbbxdrrhj.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gklimmdgt.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gowskitsk.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcukdgbi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjqhrnmmd.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gdmgsshqd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggzhskylj.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gjrrkoasz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gvrytsyiq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gzxknbzbh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/goxtzfemv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gzyounher.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpiwvfozm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gonwtpflk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gylpmofxo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gvpqrjyjs.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/glgabzsrl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gmkypiwdl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gvxtxmxtv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gegprabhr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/giughwcnn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gjfpjifdn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gnczfimib.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gfjvkwtln.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gjunwofee.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbdpjkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/grbznckbz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gxuqgelrv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gebuhertq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gzwtovdxl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gkndfzxff.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gfvqvzzoo.sHtML


<!-- 参考信息 -->