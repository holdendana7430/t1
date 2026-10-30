代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/govptlylc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnllplbb.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gdaukzdnf.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gkwaevxox.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgrrognm.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gipjoqwir.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjtqcuqj.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gozkvzmaw.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/glqbtucus.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fanxiaobao.xyz/Article/details/gzkxufwxw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gquvnexoh.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/goombpenx.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwtpfcgf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzzmopcx.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/geevrnqaa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fanxiaobao.xyz/Article/details/gsbzyndfk.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gmfezhigz.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gemyrjqkv.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaztategq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gofpqaomz.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gmnslzbos.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfawkkund.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fanxiaobao.xyz/Article/details/gxysdmqpu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fanxiaobao.xyz/Article/details/ghyrcgxmv.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvapurrx.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwwwqsei.sHtML

[A16] 真假值判断规则
来源：http://3g.fanxiaobao.xyz/Article/details/gmryxjrkg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gclqxqldq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcudpbyq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gkktmpokr.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gooecekny.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzwqnblt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glxytlivs.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gimvhsgsa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykwypqls.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gnquwvnsi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gybbyvare.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqceuyiku.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghfixaqiy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxpwnefz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gficfudew.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrzgooaq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/giwowdmln.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gtflixhje.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/gmrnvnved.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnsutiyc.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcybndxb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gnwlgixwx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gxacgzdol.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fanxiaobao.xyz/Article/details/givdmqxnv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fanxiaobao.xyz/Article/details/gcuwyubnf.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbhuyeyu.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fanxiaobao.xyz/Article/details/gohkanvie.sHtML

[A19] 交换两个变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunxxinx.sHtML

Py:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvrrultk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbbhymgr.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gafmigcqe.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdqjdqgt.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbutenlxh.sHtML

Go:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/ghikaoujc.sHtML

Ruby: a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gplvrwfoa.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfwziqck.sHtML

[A20] 读取标准输入
来源：http://baike.fanxiaobao.xyz/Article/details/ggmfwyhni.sHtML

Py:   name = input("请输入：")
来源：http://3g.fanxiaobao.xyz/Article/details/gvhdlluyq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fanxiaobao.xyz/Article/details/gvevzhrqm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjgnrjeu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslibvnbv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fanxiaobao.xyz/Article/details/glmycdmfe.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqkzbcxq.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnokanfxr.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fanxiaobao.xyz/Article/details/grtzoqyto.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glssngtve.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gextcahea.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/ggzmgqcbt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guolunqhn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjzvsyfa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gbezucfvi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gtvibsuif.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gfwvnngwf.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmfcwoxr.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcofsseye.sHtML

Py:   len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdrlqplf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelsdljnr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpysgznq.sHtML

TS:   s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gikimkfji.sHtML

Java: s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gekyymfqu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqewprktq.sHtML

Ruby: s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndvifjbf.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbxnaghw.sHtML

[A23] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofutpksq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvsjsnld.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fanxiaobao.xyz/Article/details/gjrnqpfvq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gymqnqzka.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gamfakbui.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfankasie.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fanxiaobao.xyz/Article/details/grrgzwmdf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzehvhpxd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fanxiaobao.xyz/Article/details/gwlafmlhy.sHtML

[A24] 去除首尾空白
来源：http://wap.fanxiaobao.xyz/Article/details/gjckkbvod.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gxholitmi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gylraglsb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdcpumtd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gyqqawqnf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fanxiaobao.xyz/Article/details/gitcckxfz.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnlhansna.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gveuvrkqn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gqoxxqnsi.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gryrtgznf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fanxiaobao.xyz/Article/details/gzwbvwrww.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsfcfcdz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glggnbfnj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gptorhxlq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/girkbeymb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaegrrtbh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtgdrcrz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltfuurue.sHtML

[A26] 类型转换总览
来源：http://3g.fanxiaobao.xyz/Article/details/gnzusujhy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoghziio.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyturmjn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fanxiaobao.xyz/Article/details/gdpjtumge.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fanxiaobao.xyz/Article/details/gzotvcecx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtgqjmta.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guboqques.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmbjoute.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/givyiurvr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gglvcmlzi.sHtML

B. 流程控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaajzkjng.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzcdrkgx.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrhgnird.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpdzvkxi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuljelop.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gayezjvme.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/geeogspmy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gfndbqaea.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpriwptvq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gqhzlhrtm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gjsplrxxp.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fanxiaobao.xyz/Article/details/gwebzcpae.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtsjxvlv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpdqlxhry.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzwqjwwf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwclrklhx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/girsqyjws.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnhaakin.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gwivyglpf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gpmgpbsbl.sHtML

[B03] switch / match / case
来源：http://3g.fanxiaobao.xyz/Article/details/gogejqahg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gtyvifuun.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjyprkifv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwaqbxehd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxribhgd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnojgenfv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/glpvqokne.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fanxiaobao.xyz/Article/details/gfhwiznan.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/giwotdsbg.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghvclaai.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gdpinozvm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfulyypq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsiciueg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagkjpluy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsciwinop.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkitjfhsd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/giqhfrvvz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhqbqtnu.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gilbnitzf.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fanxiaobao.xyz/Article/details/gzermajge.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaqprhljz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxhprmmp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gycrreqdb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdifmwyqe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gniiwjimt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gkfmohpjl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gujcbjuno.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejbvblej.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvsnsjqj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghngqdwtc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gitovwqfb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gatyewpdh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyepexzvn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fanxiaobao.xyz/Article/details/ggjyuauhj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gcemfppvj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnjeolzq.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/geqltekwg.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkysnnbsk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giwocdqhk.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grtujmnic.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzkeiwqz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaefpqntk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gfvqegiar.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqumyxek.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzinocxhr.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/gknwjeewp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbcsoxou.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gsdnawphy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwebszbbk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/ggnkgapji.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/guhebzekv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbnfkjdz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkewupla.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gpjjtujfp.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/glvouembq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjrdzied.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtjloqnki.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcdovpkw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmtqiasg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcxxmsue.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgrardwi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gklkedclr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqefhzcql.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/gbegwkmjd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvpxsjlu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgekfhgf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnbqorsd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjxbmofd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxnqxhcbs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmbaazs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfgyitve.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gewjglbjj.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/goezpvcrr.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fanxiaobao.xyz/Article/details/gctmtyfck.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbovqvqvg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/giuuibchj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqjbckeh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaignhddj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gjsctkikv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejygtvlm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gboujkkvz.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/grvuokudx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gaclhqcrn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/goqsewalo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gdwuzdszd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcxhlnev.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyatoxecx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfbouhar.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gdhwkiyib.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmouyqlt.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gfydreglh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvezwxmgg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gifzawjue.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/giuuyqdov.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdxmslmsy.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gdttfiwvt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/gypgubuwa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fanxiaobao.xyz/Article/details/gpyxbzuoi.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fanxiaobao.xyz/Article/details/gpagmpssf.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/gkdtskiav.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyhauvwl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnuuwkcv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcjlinso.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gryqabanm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaotkmfjt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtfflhral.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ggbcmrzhy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gktbblmgc.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwpwvajg.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqifmlrgw.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gsyfvztrf.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/giwrqkomu.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnsbpxkm.sHtML

Java: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gqolftwke.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gaurwxaii.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaumditd.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgumylfi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgmddvjj.sHtML

Py:   if not data: return
来源：http://3g.fanxiaobao.xyz/Article/details/glyfzspdz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gommfknlq.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyzboaxt.sHtML

TS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimhucjxx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkxmrmel.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxdfqvqs.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gaoxrsaba.sHtML

C#:   if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsykmuip.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjxqqajuv.sHtML

C. 函数与作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gmndeefwu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glibhndib.sHtML

[C01] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gesybgpmc.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gyvybvrae.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goekvqmcf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkcjxfzvy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqeafkbq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhapzxjj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gfmablmxr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigbmlhiq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmvdugju.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gsogfyefg.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgdwjpsq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqwfybuxw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqehwkdrc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbafxlzkz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqujatxdk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalyhfsy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntuxrjyy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbmlzlnj.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvahwrhg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkxlswuz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghcnquto.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwrctjpy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrudrxmm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjgftdrdw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gdxyxznsq.sHtML


<!-- 参考信息 -->