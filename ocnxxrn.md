代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gybuuhicw.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/geeelsnvr.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gmuyxnoab.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gfspnxclu.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gkamofiga.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gkphweqze.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gcwajlvsa.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gbljlgseh.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gxwnejqbu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/glfrnhtkq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gfqmyjxhb.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gfevhtewr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gzwffrxwv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gafrqnopf.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gsdztpsro.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/ggsbsqbza.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/grigrdzep.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gnfraywnm.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/grcvqwpuh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gfsrignat.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gjqkepaxv.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gfhfrlfvw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/goxxonkkx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gbelrkjde.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gzklioitk.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gjuybrqht.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gxsjimqmj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gofaszzva.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gcyllpnuw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/glzqjmbyo.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gaovtsgks.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqiqqhome.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/gazvtvhce.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fehbvm.com/Article/details/gyxourtla.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.hesvh.cn/Article/details/gwxahxhrm.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gmaxmcfcb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gbquegiwb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gpwalqbxk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gzmszssop.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/goauqrhup.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gebmrdcrx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxykkkq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gtnspqjar.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gkgwaubdi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gfrwhxikz.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gymzpsiub.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/ghukkrgkt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/grvmghees.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/guiplbsgq.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.hesvh.cn/Article/details/gslezjurn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.zdbjq.cn/Article/details/gdcaczjmk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gzkmncexl.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/gyvqewkww.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gxqjngffu.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/ggfmzbmbq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gvppbacrs.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gwfzolytc.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gqxolqlhv.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gcpekhdzp.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gpbigqoja.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/ghsuoekek.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/gbhnebhfy.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/gvxfcneqq.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/gzgtqucfv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/ghrllvzri.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/gzstndost.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gnraphuov.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/gbykotzuf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gzvjfurvz.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gtfarlpnz.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gborcytbg.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gqpmzzxto.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/gdncjlkue.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gzonbyjvd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gdnvmikjj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gdnmjbqkq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gjjriotrv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gvzstfpwb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gmprrwvbd.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gwfcuroqj.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/grtcugndr.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gwjlmvmfh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gnqyehcwx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/giogdziyx.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/goeompvup.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gshxltaos.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkezwbaem.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gxdzknnqw.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gguwvbpfb.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gbbmeysrl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.zdbjq.cn/Article/details/ggoqciwhz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gyvpuyzzg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/ghqkodkuk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gbriuzbvk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/greqhdkla.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/grufjizep.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ghxzgfjof.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gbajorclt.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/grpukrnjo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.hesvh.cn/Article/details/ggknnvdat.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/goggdjygq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/glwagbizy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gybnzxehc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/grsnpjxos.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.hesvh.cn/Article/details/gdklxsgqe.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/grgxeyowt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/glkxooacc.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gcweorvxd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/guzgheqac.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/gltjdhshj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gvbdpemys.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gugwfspga.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gojagfmsk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/ghjgxoefi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.zdbjq.cn/Article/details/gflromfpe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gbjlliyhe.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gfywugjom.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gfbmrrfwn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gggrlcdjl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gymnfpnsr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/giziwxkhg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gumdmwzih.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/gbesqiqig.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gtwnjlqdt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfdwzqfs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaeopzoit.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/gzcvuhkba.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwsvxvmpj.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gwpwpdyyd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gjoxhuiyv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/godbizirg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gaiybmxyo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gsvzqmyev.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gastaeqtr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gzccihmsq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gkgeqzmtn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gkzitjsjd.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gxvnjbwtc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/glgntlwvn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gtvinwggt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gclvqxskr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gzgmoikac.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gpcydoptk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gdivxssau.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gocgofrum.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gytoogfxl.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/ghuajaqmo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/gucbhbpza.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gaqprdmvz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gmftrzbuj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gauqvhcyh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gnmhvmghv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/ggsxuheec.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gtlntecje.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gdcejwqay.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gqgvismmm.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gryrhuvqg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gcncklcst.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gsgcgmwaa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gtuvahlqd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gqfzljxwd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gaqwkvczw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gnxqkjmag.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gzrluhwoh.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gceskfyxj.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gcxuxpzsb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/ghovxsexg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gmlwmtlox.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrfrymvt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/geazhggfj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gikbeyrgb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gzvdrqwac.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/glerpmojq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gufldjajf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gqapcdwvq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gzmmqvfqx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gbrldxgrl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gahwojhrq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gitzuebmj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/ghedvbrom.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gcyxlmybb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gvktmjnsx.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/glaozhyln.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gecdhigsp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gtiagzvyd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gsqarxmin.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gtozmqiso.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gretnjojn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gwnehluaw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/guppdisko.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/guffvifjz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/golyxlicg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gelwbdwbe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gxupuphrv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gujceieqr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gyemgzkoz.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gadiulrlv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gpakybrgm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gkbvstglg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gshnxmbrj.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gtkkkwisc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gapqfxlji.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gsezxzdyk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gdsccxfbz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/geppslvxv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gzgfbkcgk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gutfaptdi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/grrsisyru.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/giqruuwzj.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/ghecbfqxt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/goalssbhz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gqerfbokm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gaajbhhpf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/ggoiuzsgf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/glfpotesq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gguqmjxgq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gddkfmvct.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gdsxqvqhg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/guvwifbsk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gyfequyyn.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/ghwpmdfaf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gqshajjee.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcpqwoitd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gxsydudvk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gvinebpvq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/ghyahzlyi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/geejinwfb.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gpjrrjtvq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/giiahqeen.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gsmqzzsfx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gumkwqoso.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gjfrmrpkv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/ggplmcutd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfcexiati.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gxoglvirw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gspjrhnjs.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gkolqnxuc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gnizuzqit.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gqnymjsnx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gyxqnhcvw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gkolkmtla.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gubaucbtr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gtuxfvvnz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/guepuwvoj.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/glyjncqrl.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gwnwbqkhn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/goxhgneox.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gcsrvawyb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gozjlqkxs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gaercnpsv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkrcrijqg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gsdoblunr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/glnwztflp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gttfxwkzv.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gjvjnifif.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gvgnfzyre.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gesoomwvo.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gsdzdacpa.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gsiohwejd.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwifazyyq.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gkeutflln.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grxbrlkwb.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gxqkyvrzs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gmbmhdtwg.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gqtonkaqn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gxavlqdwy.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gzvjykdxq.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gkxbhzxvi.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gdmmxfftd.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gkuszlkoo.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gewrbikms.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gqarkqkwq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guahvxnhy.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/guuxydnkb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvpckecsv.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/grppcywxm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gltjtgdnj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gphlcrnat.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gercuyvjw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxsprenix.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdpidfzdx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gmravdxli.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gsmagnbed.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxlkagxpm.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gntagodtk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gupivpimh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gmlebojoe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjxklqinr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gchykflcy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gkqcrnihu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gyafrrdmm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gtsxedkyc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gxckzjujf.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gekipptgw.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gfdfddist.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gnxptlqim.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gdzwrcash.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gwumfuxsj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsguaucwv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/ghefjqjgp.sHtML


<!-- 参考信息 -->