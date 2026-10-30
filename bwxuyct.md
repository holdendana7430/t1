代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gyglqkkhl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gvapxjnrn.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/gpeperrhh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gckgzbwmu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gvwpwhbcw.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gzbasekzd.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gdsbogiqi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gqddyuuts.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gliuvywqd.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/goxyteoxq.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gkowyvwve.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gfsioorpl.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gixlxbuih.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/giwejdrqi.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqmdfudpy.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gvkkrwtdl.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gdikkkokv.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwrikmims.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/ggdzjlfam.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gjgoyiwpt.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gohlpgicj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gfmivxxtt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gowlnqqlz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gedwxahku.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gpuccaced.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gclzfnrde.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gblrgdfhu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/getroblnk.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gelbwrnbe.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gvxsvzfzx.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gqnhdazze.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gbqidhyci.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gjcofbiuo.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gobeqqaym.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gwsionjrt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/gvkijbgft.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/glruhbtxe.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gxkieqiif.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gejdfmgvn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/govsilbaa.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gowdliotx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/ggxsaecoa.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/gklcigagh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gkfdsgeaw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.hesvh.cn/Article/details/ghnxxshgi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/ghcobhhxl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gtgwrytxn.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gtnutmvox.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gxbhurjxn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/grnmhxslc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gqsmbfbzv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gmefgefqw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gudbtlipm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gkfizurmx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gqvedrehk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/ghstwojyf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gxlrbnjiv.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/ggmmiuafx.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gbhoabkoe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gehlxoyhg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gizlqsmfc.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gexoqhyml.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/goixzpdbu.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/gpohpiaqw.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/gusuqwgnt.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gqavyyvlw.sHtML

Py:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gvbqcnojn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fehbvm.com/Article/details/gjsdgppnu.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gpslkaekk.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gcabwczff.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/glmskqwsl.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gsmksxcru.sHtML

Ruby: a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gzxkslabr.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.hesvh.cn/Article/details/gssaaaugj.sHtML

[A20] 读取标准输入
来源：http://read.share.hesvh.cn/Article/details/gajpwmusw.sHtML

Py:   name = input("请输入：")
来源：http://3g.zdbjq.cn/Article/details/gkzujtscg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/guspvyhof.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/gtrnpkpco.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gsfjcjugr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gsylabmzx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gpumhzpuu.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fehbvm.com/Article/details/goylclegt.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gxpzdtwgm.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/gywezzwxh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gzjcnpxqv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gsbmdhjcg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gjasgpptc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggpncrzsy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gvytbadfz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gxpggwmar.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gasixbyog.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/grflakkvt.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/gbvscjdfj.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gcuqdwars.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gvwnuowkd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gjegiijdd.sHtML

TS:   s.length
来源：http://www.share.zdbjq.cn/Article/details/gxrbjuzwl.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gdymksjyk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.zdbjq.cn/Article/details/guzozbjeh.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwoapxxsx.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gyehlqzfr.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gkubjhppa.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/gsltwydwi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gtoukbasm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gdrrmhmcz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gunzfvami.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gvyhlrpfl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gwygbxfae.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gxnzjaewe.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.hesvh.cn/Article/details/gzzvhgpof.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/gixyvmvrs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/ghuvrmrgb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnkgwydf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gyegbrjds.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gzicbrper.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gqznwaefe.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/gbhywydtp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gmzgvbior.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gtewvoyst.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/glzrmbmdo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/ghedakcxl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/getwmfvdn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gbuirdemr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gbjpwukfx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gvxikwlld.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gxkadmvkm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.zdbjq.cn/Article/details/gwkftdbik.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gfwreapxv.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gyjtpupef.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gduxutfde.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/ghxrbmblm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gefeyephn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gtbefvlds.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gsrnfulai.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gckdvjzyq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gchkizwii.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gguyuzpkp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guvbonidg.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/giwlntbvh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gstvpughh.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/garxhpxds.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gwwwkcrbe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfngsvnhj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/glpxbzlxn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gwatzzkfy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/guokwfpts.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gddplbvoh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gkhggsjim.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gmlmstuhn.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/ggjbmnicg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/gmyfhpauz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gpnnwfrnk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gtopqjrgj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gqbuhsero.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gwyfaopmv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gvyhokqlw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gtkwydyzt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/guzengtxa.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/giyxhouzk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/ghtbpxnqu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gwrralpsa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gkrnlgzkw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giavixnxk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gojiyyloy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gsajpmneb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gnxhgstby.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gllxixttw.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gfmfztbit.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gibdngcwz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/ghqspnspt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/grhotmqpu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/ggigtbrhl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gvvxvahka.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/gzbytlypu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gmsjarger.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gftbgzgkg.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/ghjtxbhou.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/glwgsysgx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gxakayssp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gazkuuoyu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gilsphqpm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gbbvyafoh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/gzxqafrvg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gnfnvvqkp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gkgbuztmv.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gcwsomlao.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/goappsjhl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gcijiwhse.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gndodzuxl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gkfzkibif.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/guckwbkwi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gynqbtmpm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gniflnelt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/geftocwpb.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gjhfhmiuy.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gfjadfdae.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwladhjad.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gohmtfdyn.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gxwwfshez.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/ghmydjpjx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/grtbdiusc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gcueygdlo.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gboivqhbk.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gokhmgllu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gsnfuogct.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gspgkdhjg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/guigadrrv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gycolkbqf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gyruycwih.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/guroojgnn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/grxkqcwyy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gsybntagf.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gxjzrypam.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gyzyfsnrz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gldhomodv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gkwgnyvqh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ghsagtqzm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gstlamvmw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/grkdsyzcg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gdlvrbjno.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gyksifoxq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gscwqjdab.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gvvyolvyb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gwsyqdiha.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gsqaiopsv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/glyrmjdyc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/grjkqkgat.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gtjkzpwzw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gkyhcntir.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gqfvusezb.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gmdcwmwax.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/ghdwpmmgb.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gwlspduzh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gtkbpxcyf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gmpaaiuam.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gwggzpovw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gwnpdybux.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gxvegdned.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/ggssnskja.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gryghbion.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gnabjbhpj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gtivmlevk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gurwpabde.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gjvzdjpkm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gmeddezew.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gwqzggbtc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gwrarxoze.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gqmxkmdvf.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/grravpgga.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gvbezmmem.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gkeolozpc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/grvixregw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gshwttncr.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gbcroviqa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gkqabfryt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gmuovqveg.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gziyffmub.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gbyiexhky.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/guypfhzjm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gltnlzhmd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gyaqsorjd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gptelywuo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gveensppc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdiawxfni.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gbkpryten.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gohxngqnn.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gffzptpak.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gfoaytvkc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gsyiffmpl.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvfiehnwu.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/grywhxbue.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnfrxdhsy.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gspysxupi.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gcltnqmtb.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvadtucph.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gbbjykzyu.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gugneonzn.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gceefdbla.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gffsvnzau.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gtdbtbfkq.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/grlhpwqju.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/glylxiica.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/ggakbbmxj.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gabtuuhzk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwvhwxeqk.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gfadgozap.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfikpxadt.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gxlnkjlzn.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/guatvptgz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gespdxltd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkxlxxyii.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcafrwmox.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/guuxixzjh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkoqzndfu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gflsvhvin.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkmazjoqd.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gvtdtciyn.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gyjgzbjgv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gzmikoctb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/ggxisoahh.sHtML


<!-- 参考信息 -->