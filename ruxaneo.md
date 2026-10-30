代发 wailian999

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gbctotltk.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gwvovdmus.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gdmmrwayb.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gsbzxqerf.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/glnfirezu.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gduufwbxa.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gwccklpxs.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gmnnssyum.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/goxjhnnlh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gflovgfio.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gnmqfwtry.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gqdzxhzpu.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gnzhdkkre.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fehbvm.com/Article/details/gsuspjyng.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gzrxqjzyt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gejtxedyh.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/glfqbjrrb.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gehkmnvqz.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gbqwrjodv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gxzclovub.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gnofwwnyq.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/guuvwfdjz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gphkghauj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/ghqtnnvtc.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gpehlhphe.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gtwbrxijs.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/gzgsvtscy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gbhourqtc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/ggaunwhre.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gwuqkqoui.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/ginqoskcx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gtsckddap.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gwctilqtv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/glfprhomh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gckmcdhng.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gnpxscbri.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gylyyqqji.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/gwcnjlado.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gaqceqwcc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gvnwrrclg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/giyjoiazl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gzwvooufp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gvauselhe.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gmlgmgbmm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fehbvm.com/Article/details/gqyazhtks.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/goxrmvugq.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gedvhqzjm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gseryiqvr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/goblkyrnw.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gggqmwfex.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/ggbuggtwx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/goysvidry.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.hesvh.cn/Article/details/gslyjvgkt.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gcdpzredh.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gralrzudq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gqtymkcxm.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/girjvblzq.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gkmrepumu.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/gjoemxkit.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gmkxofkvd.sHtML

Ruby: a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/grldgehqn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fehbvm.com/Article/details/gppqmyxkm.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/geegsyywr.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gjxcsgoof.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/giyavmfzt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/ggqkvjrjz.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gnskskcdc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gujnwvnxk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/glimffonk.sHtML

Ruby: gets.chomp
来源：http://baike.hesvh.cn/Article/details/guucdeajx.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/glrzlfqfl.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gzjvqxwek.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.hesvh.cn/Article/details/gvvhfpsbf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gtzbdnxuc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gtzqigtnz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gomolrrpv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gssbpouii.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gfsmxgvvc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gdrpbkyme.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.zdbjq.cn/Article/details/gthyjwhgj.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxdceksll.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gdfwruszv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gogjnrroy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gwzjicuxe.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gmxhzwzbn.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/gbfaeolfo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gvgdkjkkx.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gexlyxtth.sHtML

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/gfaartyzz.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ghszyrkyx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fehbvm.com/Article/details/grbnnsckk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/grbmfreag.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gfkqlttmp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gfnfvdjcp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/garcavpbi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gwjgaurnb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gbymxlzkd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gaazjowte.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gpkopgjzb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gsykdglej.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gezxkxtbe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gabirsrvy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gvuvjyhbs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/gyqonkijd.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gaaqgsyms.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gcqwwjwqw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gjoidnixv.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gogtzczzv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gblmdlqof.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/glksibigp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gkpmpddxe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gqvkbakwz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gieioqxrk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gqxddkwra.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gepxvpqgu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gdqigzyir.sHtML

[A26] 类型转换总览
来源：http://read.share.zdbjq.cn/Article/details/gnormhzot.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gcjycgzzw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/gzrmzuhyu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gheadufjb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gkgjbpdhv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gjyyylwhj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gmxzuwwfv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gaosmgrvj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyifkeyu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkvyperxh.sHtML

B. 流程控制
来源：http://www.m.share.fehbvm.com/Article/details/gzasxmneh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqoawixge.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gbnccfvup.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gxgwwwrbt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gswmebnah.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gefllotbt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/germyrtrh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gnlyomjdi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gzzmwamyw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/gizhlorak.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/ggtoaoagu.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/gwgqocbzl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gkznqeass.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/ghfwteqlc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gelqhxezi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gnbvphura.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gfmgejdtw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gggfyraiz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/guypwmpvx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gcnvibdri.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gktiyskbx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gymgqqhan.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gmgezqeoj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gyndyjzku.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gatmzapnx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/goyihcjig.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gfbwlvrmn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/garixowlw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gzcsbdjnu.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gjbizhrzt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/gnlwmtyut.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gitmaqzmp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gsekinmjv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gtpiejnil.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/ghkfaysdz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gnqfotptr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gtsnnxpds.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gxrfjxeoe.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gyjngndtk.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gclbqomkb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gozyftwhl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gwsnbsucy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gqxuqsckm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gqktajdyp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gpnzxkihj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gyopqyktr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gzkvbtfph.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gtfokzzxf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gtpolucgx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gucnaepfp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gtvkkrutr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/guezkyvzx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gnfpnpzbc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gdhjyzmha.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/geydjchww.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/ghacdbtyl.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gfpciskty.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjkuriely.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gtewpabgg.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/getaqnwlb.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gwxysvqnx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gyuorazhm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gymfpapfh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gflpyqdmj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gsudtqywu.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gepfiziyr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gaabftrmy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gczyvrryu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gffsqqopg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/glldinzhz.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvenbcidf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/geztsgzes.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gnvhfkliu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gedtmmzms.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gmgfdrqom.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gjdczqzvo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gclvsqgtx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gugryigdx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjhdnajs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/giwaalroo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gwjhiftjm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gwybmuiet.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gygiblclh.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gozyyjzzk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/giriqnwip.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gqdmqjizv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gffxmoyrp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gpktwpxsy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gcshxgujj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gmijlmpgh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gjmyhiche.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gdcxgvaip.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gqyflweyu.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gpclebchg.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gborthaiy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gkzalsbqr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gnveopafh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gfoxqlxop.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gsptbottq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gqjxmdbby.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gagxxkjcq.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gtxaafhji.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gbtyedjya.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/ghsjtzsdr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ganifldiw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gzgytqpmj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gvijnplxj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gyylnjjte.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gdhggxluq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gxkribvty.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gqpiacjha.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gkimsarlo.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gshlrkyhc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gidioaqll.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gszakciay.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gxnhyabag.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gdyykvowz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/guathxebc.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gltxembwy.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gqsdszfog.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gwzenlhdl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/goismlhix.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gqhcfrdvt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gqaegrfln.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gomnjjudc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gkgizthez.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gbrpbqszj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gkuhuoglc.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gquzwyksk.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gvmovyqva.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/glnydqqmk.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghjnejaph.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gsrztzicj.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gchjexgja.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gnkamtdig.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gxxkwtffy.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/guadathkv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/giyrwjger.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/grcamawsc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/goslplsdk.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gwzdybqhu.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gpsggcwab.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gqsnfggxy.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gqkddirrz.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gfevvnvjg.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gbtuvxgzh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqkgfwesx.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gqxaukzas.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdwgbfrzi.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gpdssmyqq.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gogqvfidm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gplcexkfd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxoqqbepr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gkqmazcwo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gplophdjp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gvntajavy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gmqajilwk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gemekxxks.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/geyggpvst.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gltqsashr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gdikombjd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gkymtdepg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/ghlrkdjza.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gflhzwxlf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gkfstfssf.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/ghdfhljfp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gqrdogslp.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/guwgaozuu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gofxqjvty.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/grsdetqna.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/glhjzfvrr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gutelqfgv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gibzrhiqr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gvrglukkq.sHtML


<!-- 参考信息 -->