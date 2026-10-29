代发 wailian999

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gzbslpwee.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gfkhkxlzb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/glabgojej.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gbrrpszrt.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gkamsvdyy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gzafcuddg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gpmyfbmmk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gspjoyawr.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/grvfxmmwc.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gnlyxrwlc.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gbdkkyfuq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gukunkyvr.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gfswwdiah.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gbxmvgfoh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/gdoayfrzh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gojwyvaqb.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gbmscrwbe.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/geqejrguo.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/gakzbgxee.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/gvwwannpt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/gendxooml.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gliakescp.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/gwygvryue.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.hesvh.cn/Article/details/gpyqhhyib.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/gzpgxmwte.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fehbvm.com/Article/details/gsekzmaly.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/grantatvs.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gqygsjbdu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gmxabsanx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gczglxzqv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gbnpnqifi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gpxjqtanb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/goqabyxmu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gizgnovog.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzvrbiwcl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gdevxnlnj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gzmbibdxu.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gekkmbnwn.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/ggiahzrsv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gdrlsorrz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gmzdkvszk.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/grfzstbwc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/gitiolpek.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/gupsovdri.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gzpunwzdh.sHtML

[A19] 交换两个变量
来源：http://read.share.hesvh.cn/Article/details/gbezlntnj.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gcgylscdq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.zdbjq.cn/Article/details/gafdtpbhv.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gjwlryjkq.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gynrmpvyk.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.zdbjq.cn/Article/details/gdutlymop.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/ganuqtgof.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gjggyslrl.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/gifadazla.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/gjhupkhnl.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/gwhthxrxa.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gbrguxbku.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gnmgrluff.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gcvidzwot.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/ghayqldwj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/girsknkku.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/gilrwzfmo.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/ggbsaqqol.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/guovbxunw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/gokyvusvd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gpcmocvip.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gqewynbgs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gyphartrm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gdtbkxkml.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gqhdnupdi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gikluyfbh.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/gxtslmokd.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/gyuizilvh.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/ggyfozqbz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gmnpszgop.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gbyhcaked.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gpiyspejt.sHtML

Java: s.length()
来源：http://3g.hesvh.cn/Article/details/gmabteokb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/gxmllurdq.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gyspeeaez.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gtxkpocfg.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gvlutejor.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/gauivyspq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/ghcwcnosh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/glwaivnyq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gztadhcuf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gtlzgepbh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/geyysqsxe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/girzvxjps.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/gwdvoseqm.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gkneouzuy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/grkidqnxu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gxstyrpfq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/grajyilkj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gwjtvujiu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gdfyxcvrs.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/ghstcpfmt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/grxjxvgjc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gqxbfspyi.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gsyskgrkz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gmvatmklg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gmbkitahb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gioyjeted.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gjihcmeny.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gqfnusroh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gnraqnpmj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/ggogcfeot.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/ggrbjoozg.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/giakmesdo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gyjjfhgxl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gheifjjfr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/glrbclrwq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gkdxifedn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/ggcgyjund.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gzuplmbaw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gohhncvec.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gbqgddtjh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gheubykdt.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gckbvcucc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giwbdqboh.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/glbpzqimm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/glspoeluy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gjzxetegk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gevboteuo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gqzgobxli.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gspnevngm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gmwlkifse.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gnjfeesky.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gkybtoefi.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/gartqprrc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/geuxbtfel.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gthnjvuwe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/glimbjfgh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gkodyxqys.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gvatcjiet.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gfjnmogim.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gsytylvib.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/guhutqwrv.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/geeyvnehl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/ggzpkjhjn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gacedzrzh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/grwkfdfye.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmvljebkg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gntnwwcys.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gpikbdnof.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gklozlfic.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gpvhqmblc.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gawfscmvq.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/ggarviuyt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gprumxinh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gzadwfmsb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/ghklwrucd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/ghyxihfgw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gntjfvhvi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gwnpdvcge.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/grpmzrwnv.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gvcguchjc.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gipitqsiv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gacrlpvah.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gwpcdlqym.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gytznzujs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gpytwwozw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gbuwqxnoo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gaysrgkxo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/guobhxsxi.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gacjgqpsa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/giasodnij.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gpamkysez.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gibfmidzn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gynbxytpi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gesfrtjse.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gmlpzunzf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gbcrjqpzy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gutlnxlod.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gjxjvjqtr.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/geqicktbi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gobjppqzj.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/goytcksnn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgxzexy.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/grtrqzhvg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gpyqoafwz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gvwgsfqdn.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gijhaqtun.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/goojyzurc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gdtrepxfs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gmyzycfbs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gmexfcgrs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gpiqkajmh.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/geumyczrb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gzjaoworh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gdhfhjkux.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gpvcgfgeh.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gnymmgjxj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/girlnpifq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gabcabmca.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gjdwozocz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gjijafdbn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ggbjymmqm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/ggwyoiaya.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gcpupsofa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gvxkxosbf.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gxoxpcezf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gftmanzoe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gftkdcmwd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gcrwunzdw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gvkuuhfkx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/ghlnfaiqk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gqdqmkbtt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/giybqwvlh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gxozdqrig.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gyfhpyilr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gfgapdpkv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gemwoubyz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gfkdabwsy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbedlbokk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gvmbekvgw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gdecdjdlu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/glsujrgfz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gccmkxoop.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gzmwxcjsl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gihuvbarf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/goctsnmws.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gjqwogtap.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gdklfhekd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gxxntxybs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gqbwrtvqh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gbnvlhqwf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gssyvwzra.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gnhvsnohf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gqmwbgafv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gvkigyflg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gwgblmtnb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gxawrioei.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/grqgucujw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/giueoglwp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gmhcgohed.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/ggahhclms.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gwcbgrdje.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/griijwfhb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gzuchqvke.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gymrriisj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gpsbtswjq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gqbdrfvzh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gqsrqmgkd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gkmvuwjgq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ggaqfrwmx.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gcywqrecd.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gfehkfzgo.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gdeaakhov.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gdyrgbsqi.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkonylxdt.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gnezsmiru.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gcenzenqs.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gsjjxeysn.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gcqnwvrwe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gxconltgi.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gfmyafenp.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gzpyyqeep.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/glqdmkbix.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gsawxyldt.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gjnsscsmt.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gbappqekl.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gkiknwrow.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gmokhcedl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmdutjvif.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjrwmjbpj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfrvwledw.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gfotfvvhz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gcsceslcp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gyekvjkvm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfswjwahy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzvjpzqla.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggsggmxyj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gcqgkqebt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gkrbtcnzc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gadlholfm.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gntjlampo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gphhhmipk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gxkdkgayb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpexpatip.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gkkvwldwr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gteejfbjb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gndzwftfl.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gyshkntzy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gtzfjncjn.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gdkrntudb.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gsemujwdo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/grkualhut.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gmodikkbv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gilwlbnoc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gghjcibph.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gpktgrxzs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/ggbjqough.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/grmirotvb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gxquyhplw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gjmkucnkf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gnjqntsko.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gnkjeakxa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gbhfoqcaj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gebjonups.sHtML


<!-- 参考信息 -->