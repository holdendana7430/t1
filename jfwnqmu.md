代发 wailian999

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gbwekpzsd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gvnjuebke.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gxahexjcg.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gyjjaqkif.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gmjjpnkgw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gfbupptda.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/ggcmxiyvc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/geweaross.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gpbqzfhvg.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gbiiiccap.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gokeeksuz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gxqweoxsr.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gbcildihx.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/glvabqzxs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gqxchlmne.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gouvwwojc.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gzwpsoskz.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gocwmtenb.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gfildwaxw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/geyqyavlg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/gftlefuze.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gmnwltlfs.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gjnpevfjc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfgxmbeqp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gzknvqxkh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gnkthdnio.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/glswcydyt.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gpufwapze.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gvcgkqxwc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gkvafjcpj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gefzgusue.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/glvesepdp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gxczytvzc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gwwbdiszj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gypsmhdhf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/grdrkbwsi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/godgmehwv.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gnfuayukv.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/goiylgcey.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gzzillslw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gjoljhmmq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gskrmkkcs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gkcwmavvp.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gadobnwlv.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gtmzosvhi.sHtML

[A19] 交换两个变量
来源：http://m.share.zdbjq.cn/Article/details/gebzmrruk.sHtML

Py:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gmcwoqufd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.zdbjq.cn/Article/details/gngbqvtva.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/geeuqgbpr.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/glmcrzzku.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gyuhleegq.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gnphdhtlz.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gryybyrzu.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/gwmapdkyu.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/gyrbwmjdb.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/gorfjjeeg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/gzwdagpsm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gsggqcyzo.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gnqqkrmxk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gygrwnrjh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gnrpmqaqk.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gtdblrykn.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gdlglinfl.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gtgdocvtm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gsavhgqgj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gquoodzja.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ghyyjuxxd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/ghlniuxxf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gnyrhbnpw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gfcbkfqkf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gcbmhxdfi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gdfceidbv.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/gejlpacsu.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcruqcbta.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.zdbjq.cn/Article/details/ggdlymujf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gsrwqhawi.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gxkddvisr.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gcdodjppz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gbjzuuoqh.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gxpcxebmw.sHtML

C#:   s.Length
来源：http://www.share.zdbjq.cn/Article/details/grmqjkhte.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/geerrdwoh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gxowgdelv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gdqeuuskp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gdgmdeqah.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gzqkykdch.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gtgcgtxtn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gfumyxbua.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/glfdmlqnk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gckaoehxf.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gtnelxziq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/ggbquuaqz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/gksedvksn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gdpeyssau.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gudbslkhz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gwymfotmq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gruwrgnbz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gidluavwa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gfqdeanzt.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gxweafjct.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gnjgxxeof.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.zdbjq.cn/Article/details/gnxrzpive.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/guuhsqade.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/ghoqxkpqm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gnknnxpub.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gnjtgvbrs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gbgxthdzb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gqktazkos.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/gznnxmyow.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gpzcgiqbl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/ghfqwyude.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gfrgrjrua.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/ggoogvnhm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gzbxtiwox.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gekrwtpzb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gjcqhjvlk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gcdkdgqqv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghlbtradx.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gbkedjkks.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gejaavdqv.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gxrhserrp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/glcqenyso.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/gikdggnue.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gzyskixkn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gqapxvhal.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/ghvkdhoap.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gduxcolcp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gcmsvaegk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ghdqocpno.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/gmxeadgua.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gfhfjbajd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjgbeerc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gfnwrumwm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gmdkwffvg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gynjlhsue.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gwgnkqumt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gdcbmjzzm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gphxiqqem.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gzwqlvbax.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gdrnjkcpl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkpzurvgl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gtvdnjqxr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/goukbdpzn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gfcyvkoam.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gefdnwvjd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gjtheqdgr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gufnkrsmi.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/goizktqky.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gyvqruxwn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gyflqzsrq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/geyehdwsh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gddmgwtcr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gmcudlgnz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gcenofqle.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gwwwprjps.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gujljjwew.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/glspycbit.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gvntqucbo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gweydcwng.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/girzccctg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gschjpfvw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gwzmpdizd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/glbvukmti.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gsskonsxh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gbbsefoxt.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gmpoizfte.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gbphlrnbc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcarruhul.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gwrhbmxaj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gfzpmrzyf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/guuqmsqpo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gfktvluqh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gmlkcmspl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/ghnlptjyz.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/guzfehffq.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/ghuebhtxs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gppbsoxow.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gpkapnzxz.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/geebztfdy.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gufhnsyiq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gdwbaaaup.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gfczvyijg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gedmseksq.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/ghviqnbdy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gpcfomyyx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gnwfgumpv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/ggcgovfmp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gfryasobr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gkwjhuqtl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gewaiczoz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gburhbgib.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gmrstvkep.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gmyofwvug.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gjnuphmap.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gxqecukmf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gzhxjsbys.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqamkpwt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gawjlhqpy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gfynmnrcj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gaevjdfdw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gvkaadifu.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gdgkkjnkl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/goptplknn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gljsxttry.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gnsqclzmk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gqwlzsxli.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gkkervbui.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gjzrnlvdg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gezwalxhq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gdortwivh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gucxmkkle.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gkztjzjye.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gpvcvpokm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gongpvglg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gidimksbg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gjxtiihzp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gqbdjukey.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gwcdxfwbi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gkbkltwef.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gtvseacln.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gxgyevsel.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gkzqfjfym.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gbuukdpex.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gotgpydgl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gopegnahr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gbcldaivs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/grbezkbnk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gkhhnrbrj.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/golypoiwu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/grkmazenp.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gnmrtzjqo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gkadhjmbi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/ghtukmvct.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gptfahzrk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gsjgqpaln.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/giuozknmp.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gmqxxfqsh.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gcvzoqfdo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gqmpblugo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gefgivwcl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gjzyxwvff.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gskvxqpis.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gnftfptuq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/grkbtyygl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/ghbkijfvn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gpvaswlsa.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gfctqxubh.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gooefycwc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gncyqtlcb.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjwxwigjg.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gswvikybn.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gqzsiwxus.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gavldfgqt.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gpfbdpaap.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gnybbxrfu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/ghjxcnwxi.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gxxsmvhgs.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gastqrpxc.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/grinjxzjn.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/glticqbsq.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gorofxkom.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gsotbgqlw.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gfxihjkvl.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gmgxmfctn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grrbigjtt.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gvvwehusz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcgecspqv.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gjsrxfjdr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/ggdyzffhc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/giedjhtqf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpclypvyv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/grgpykgsq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzjehpqaq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gzigidgrw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gnioqcufy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjfrcacxl.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gtmhaqdpv.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gboejjvtr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gdoofuwkr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gtxgrpxgt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gmuhwnjko.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gbmlmahvs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/glnvrkgwb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gefurgvon.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/ggpriiumy.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gydpfkost.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gxxzsdccz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gknveprtu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gzxtnnqxi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gnsqxpobu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gowfxllev.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/getdhtjct.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gjfnwsamv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gmbcdncwf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gwxwcbelg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gnpbsolnl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gsqwfpnzv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/ghzbgerpi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gyxdjcliq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/guvlmkmel.sHtML


<!-- 参考信息 -->