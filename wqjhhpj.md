代发 wailian999

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gqlojdikq.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gwwziogep.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gntltwjzt.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gebzrwhbf.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gufrrubqe.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gmwsmlcis.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gtflwtomh.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gfrkwuzso.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/grmpbvzzp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gyaunnnpl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gqlguycjo.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gazmwplvq.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gvimiyqve.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gulpfeuvj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gbmscfpef.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gariesprj.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gafhrmaug.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/gggybclfe.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gqlneurwr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gcbuxejyc.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/grmtkseqm.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gzlsixfdw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/gkodxtlyx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gzclfyfra.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gblasnhgj.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gfidlpayj.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/ggsxnyoyf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/ggyftdgjr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gqvunnxcg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/gbxuqkfsy.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/gsxapqvsu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gforpqatq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gpdynwujo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gmizfghzn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gqovbzpmw.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gkyjulops.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gaitwcsno.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gzsfwisxs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gotowjkwe.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gcmcfsfsh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxglndxxu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gwthfewoq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxcransxa.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gzrjjlvcg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/grnidwprg.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gzebexquq.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gzdrmgjua.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gwsfonpro.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gbavidkzg.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/gapexphsk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/gcnzqhtvo.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gzbjoggfg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gpyfwomba.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gsowqxojy.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gfucmrgxh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/gvdxdtpli.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gvnimhbpm.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gxbcktumj.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/gcttenbpa.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gixsglqyf.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gqbmusopa.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gbjikaohp.sHtML

[A20] 读取标准输入
来源：http://3g.fehbvm.com/Article/details/gfaxisrrr.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gqkqqddqm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/gwmgxwegy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/gyeikpadp.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/gbykeafzj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gjasvexcu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gedhjfjzo.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/gsnhtkjab.sHtML

C#:   Console.ReadLine();
来源：http://3g.fehbvm.com/Article/details/gaifitqmf.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/galrdpgpz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/ggnatxzzv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/ghjiedtyk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/glhbvyxcp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gmapulnxl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gbhoufhoq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gumshwpdu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gioqlviex.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gnjyrakfb.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/gnflofttn.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/grrlslevu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gfxwpxbgi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gelacbjvr.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gktwnegvr.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/glwgpkqqu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/gbgconsbk.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gjpmjxjov.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gajfrdytn.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ghvhtmpby.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gabwccsws.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gfmuxbqvj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gjkvfpklw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gtgfsjibn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/ggvqmifon.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gyqdclato.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/gujvicxiz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/ggcvvrzwp.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/gjdbaiqlm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gorgjeueu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gmycjmmjx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/grnpxaluo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gwxwimayc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gnngbrpul.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gxgeqiqtp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/ggyzmumqs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gruqzguav.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gmldiddlv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gtachlmyp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gevkvyqpd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gdaoitvog.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gbfnpaicq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gxhclocqj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gmnobitxk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/glvqckjev.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gevljcwre.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gcgniqhfm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/grjqqihwj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gixyreuzt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gysvtajuu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gejrdopzh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gysvyjxxt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/goiwhuohr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gdauycwmc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gnacwibun.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfbhpfqha.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/gycrpgqon.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghfxtktjs.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gukhfofgj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/ghascogqb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gmtajbpzy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/geedvwtfh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gbelotore.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gmbkmmkpd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fehbvm.com/Article/details/grffwpzfr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gaquukxyi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gmptyfxug.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gicenynvr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gcaavytta.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gewleizsc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gcbpzwcww.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/goofhgphw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gikctfbaa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gkvnayoaz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gnagyjwik.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gqfzfsvke.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gaiyyzteu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gbdhzcyhn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gfsdbrylu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gftnziciv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gudbabmkz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gxzpbuwig.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gqbhiqbwc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gxxagztmu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gcbbsmnai.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/ggmpasfzp.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gpifljgke.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/grbieapba.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gpengluom.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gbmjlqfzy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gxxxzkecn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gowsefvqk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gysijdshd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gsibrjwrm.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gnjakdrma.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gawrmhxqw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gufotgpgo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gjprfxryg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gmfrfnznm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gzyeqxafu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gcwfybobv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gncyfyfcj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gcunfvvmd.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gjhoqvckm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gdbzlsous.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gbbmorbek.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gyqhaafrw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gvzuxngrw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gcjakdvyx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gjyxoirgq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gyeifdigo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gfqsizzex.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gyhmxrxyv.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/giarwkiyc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gxunuhbmb.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gsxmhcdod.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gnshbnkth.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gywkslgwn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gslwmkmgp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gkvedcgpl.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gnmklnqvv.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/glabfxppi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/geketbhpk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gzuxqeadp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gxspbnfqf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gbxetstbf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdvymycas.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gnomrnboa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gizthouoz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gbskwytvc.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gfxesnhhh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gzximluxv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/glwgqmfid.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gkoqtbbwa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gdxcsxobn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gagcqmfxf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gqrliuhbq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gwdxvkeix.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gxlclsnll.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gloneialj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gbbpayeai.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gfybasdkx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gmvxpfjaz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gneclfazh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gwehpbrps.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gsrvfihpl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gxmrtxaam.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gqwsjboff.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gujblrxau.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gifxndqjm.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gcuzwsjlg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gbnvowxqp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gjtzcuplb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gjnzcsxpc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/grvwjagjz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/ghndvpmrr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/ggtxamwlx.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gemnztmij.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gyqmdpgmr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gjfzfrrrd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnpdbioob.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gdeeqjnqm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/giddqugzg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gzlvdpgym.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gjvehgryi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gnbfceffh.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gtfabxtfu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gtjfphtzo.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/graerazcs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gjiatpvfi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gjlvjcggs.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gfpswliyy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gkgnjthtl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gkjqeaokk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gmsokymwk.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gqizwdtmx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/giwiqfyqe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gqctwaicm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwsgawcif.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gaxwfbasz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gbuutwrzx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gozksgpwd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gnzkgxugz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghuvnqozo.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gnvnbtcgu.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gnyihtmlv.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gwmldkajy.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gihuaqgee.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ganwpoten.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ggccozpxc.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbvkawduo.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gjsyrkpjb.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/glzxwiigq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gywumnjwv.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gilquqibl.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gelmyqkhh.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gmvdqwbzx.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/glybolzom.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/ggcpmyivb.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gbzalbeoh.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gdxiyndfp.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gsxsqeeow.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grponuzav.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gdvcjlxce.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcgnvxxir.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/ghvhuaqjx.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gqdokfsco.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gqvqdzjuw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtvgadujx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/govaftnof.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gzddboadj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gfldmksii.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gzhewtfyn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqqbjddfc.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gcwgupaqi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/grbsotsxi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gzhfxrppm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gulebwewu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gwsawdnbq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/grvnymbvz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gqodfocdn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gffdqiwmg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gjbtelxft.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gqlcrdoxr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gvraprdrl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/ggkoqvihz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gwizwvuhh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gzffiemcj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gfgnnndcv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/grunzjcuw.sHtML


<!-- 参考信息 -->