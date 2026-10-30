代发 wailian999

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gwyvgwxcl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/gwqlbrdgq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gmlrfdmbi.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gjxtitajp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gwdistfjd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gurbqgmbd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gccgqwczt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gdahapbfy.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/grhhhciye.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gcyycgelp.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gvpkuphoh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gkgdkppxp.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/glisbbaec.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gighwtuqw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gyzasfovy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fehbvm.com/Article/details/gjpujfaid.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gydegsfjl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gmtnajsuc.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gepyoitdh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gdgckgdko.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gnutidzhl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gxylpiibb.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gvffmmeud.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gcfvfryfv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/ggefrdjun.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gslaevhym.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/goymmkyar.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gvkkapgzb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gxgduebdb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpagavmed.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gwxzptnnn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/guwamolif.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gifljppot.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gocffmdyc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gvvsnxtcp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/guoihyzva.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.hesvh.cn/Article/details/glcezxutd.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/ghdiejdqh.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gkqyayibd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/glzfmydtm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/ggtevrogk.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/ghutitnmk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.zdbjq.cn/Article/details/gyelstcad.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gtiaqjgsa.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwhxwfw.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gamuhxuds.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gdhyssxgu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gtepzkomo.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gintkfvum.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gsmmcrsvx.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fehbvm.com/Article/details/gdwldlvbs.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gxddzrrgk.sHtML

Ruby: a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/geikaqatk.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/gldpamuen.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gbydxrpjd.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/ghvlhfzqd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gruwppbtx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gosdmzxoo.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/gxrjfivyi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gepovodaz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/gqppzyvbs.sHtML

Ruby: gets.chomp
来源：http://baike.hesvh.cn/Article/details/gqniryynv.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gdtptbzze.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gdacngzys.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gwgwwkoxr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gcqebuvvu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gmxljoykd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gkivfczmo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/glsjtofii.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gggxnuhva.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gsjyhzvhf.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gwrwcwovs.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ggwamunvw.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gcqmxusao.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/gvbgtfjbd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gfygpcbrl.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/ggcfezfmb.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gthgctqjc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/gcqiuwpxn.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/grvliwerw.sHtML

C#:   s.Length
来源：http://blog.fehbvm.com/Article/details/gfyrdhxnt.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gemsficun.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gvpxkftpo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/gymacxvxa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/glpqshlcs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gkxuvdqfr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/goqwijstc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gclhuennc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/glejgaaoa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gsaitybbg.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/ggvfdogvk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/gohmntlcd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fehbvm.com/Article/details/gbxpcwuau.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/grpgypabz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gshduzpws.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gtzdiisrd.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gcodcklgl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/giwdmhvle.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gqvjaieiz.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gpycjveln.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/glcevismj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gfmtbrjav.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gnjggmpau.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gpdeecise.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gypenzgde.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gvjkgdzky.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gtebhngds.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gtxcoyyhc.sHtML

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gmiqykooi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gxhwtvrnr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gffdzirri.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gbcayeoeu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gxdabgvhk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gmmjjqbos.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/ggtcpcmrv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gsllabzvr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzvjrdb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqvwamlpc.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gmcivuczw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxjtsrjq.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gmjzfscvv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/gbtyvasfb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gxrqnykeb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gaflxzaji.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gcztvtnwt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gpclbjczo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gfjrvqybk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gjuqktcdi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/grflqxlfz.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gcyimsidn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gpdokhokj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gnvgkbwbl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gldvfwybn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gejsjljcv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gybdpfikc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gsawuoncx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gclbkddvy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/grrypkcbd.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gfmwzjocw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gdrpumuqk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/goijdvxdq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gighcyeaz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gokyjexud.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gqsywvkhn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gbnutnqmc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gfvjxfkwg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gyzyqdvrr.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gbroucpyw.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gvgcahwbm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/galwcxphg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/ghliiuaub.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gwesbtifn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gghqireby.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gejjjocss.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gickxszbx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/ggpsodebi.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/guawbymfd.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/ghjgpjmnl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gvubfcann.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gewiizluy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gdkwzjfbw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gqevvpfku.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gkzkxwrih.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gxlgdexol.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gtlsgxema.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gahezpykb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gxdiacvgb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/guekfxeux.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/glzynhhhc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gfzcgqdtb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gkvhsmeee.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gsomtlxcc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/giqwkaglh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gzklfvplh.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/ghjnoxlso.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/ghbgarmti.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghrnaachq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzwanmdez.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gfgydrxtd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/ggzaqrxfw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gnwletyxs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/grkbbymtd.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gsjaumivn.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gcnhxedpo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gcpfjaiqf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gjjsolxce.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gzujcnmur.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gquptiasd.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gibjlqpxg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gubsawjdm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gbhcoiaru.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gpldpbhof.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gtdqmkkbk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/ghiibanko.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gertrshqk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gvxvvszdw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gfsddyplt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gixnofwyo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/guodenfgh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gvihqwoza.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gytnpsoto.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gxuqumknn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/geavtkomm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gwplplhtm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gskbhpttf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/grpoalngy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gbachghwp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gzvnfzsyz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gqwkdgxdv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gzhloloaz.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gruxdczdj.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/ghtnjjggy.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gzwegvghx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gnnwvkjpu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gcxkvorab.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gnaleitgn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gpnqwuwda.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/geldilqja.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/govqfjwdu.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/giljyssmc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gezjfvlar.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gqvujapto.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gmgyivxpm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjumrtgsn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gggronfjd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gsvihsozy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/glulaukbx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gxumgxgmf.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gymuqdtwj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gghahbeoe.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gnydooqbc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gsyublefc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/grpaeygsd.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gajnmlejj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gouhzkhxv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/ggdgkmkqz.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gwtfvvdnf.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gtcectjoh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gpaxzqffg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gahglbzvw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/ganooidwk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gkunfpskf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gfaleehem.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/grsriuggo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gfxjpmhtq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/glzwyttao.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gfegmnywa.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gjmbvcehb.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gbtryufiu.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gfbqfptfs.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfzexgrmw.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/grjslhiej.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gqctlbzhd.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/geffebinb.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gveprxmji.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gjhlmcjsz.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gkdbxkoos.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/ggwlyinoy.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gotomnwyr.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gxwgoterg.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gpvsjjyca.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gltzhehcb.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/glkjsdpuq.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gohboclmo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaqtzsgjw.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gvgmixkda.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvtbwnltg.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gwbjlntyi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gdheologb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gggpjbvnw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/grclbontn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcqdxtcvw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gjigifaxb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gqgdqqkjb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gddohqpmn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghdvdbnod.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjskaamkb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gymbspdpz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/ghcweinpk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gexpcmpid.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxhknnrem.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gkymkjbup.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gjviqfrrl.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gtczenunm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gkukgmbgr.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/grmxebrxv.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/grxpgfdsv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gwicxjzqo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gjygzojhn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gdqaiqzdk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gnihxrwiw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/ggcuehhcm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gpdfrperd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gzmujawhb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gfhtzdagf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gkhadgjby.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gnwdwkxcm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmyaubjne.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gyyrojjcy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gyiiqmrqv.sHtML


<!-- 参考信息 -->