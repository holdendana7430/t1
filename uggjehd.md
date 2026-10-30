代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/guhvhperg.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/glosgvtch.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gbcxufaby.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gtvorqdiv.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gtkqzdfmg.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gookhpdab.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/guowivmhu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/ggdrtrgyt.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/gjemfbwrw.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gqykztghg.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gtojyjukx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gsyqlzkwp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/govgrdlrw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/glsbsaqjs.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gobdlwghq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/gxhqixbbt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/giohntryz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gnzntgmdk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/guicoyiwl.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gdwqbcaag.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/ggsmrachi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gyybipvjm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gxskghxyq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gdmpoihqj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gduhnzbxt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gwoeoalkm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/guhsfqiww.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gbixaeski.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gkfpqncbd.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gahtixtyi.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/guzbkkrsh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/ggguxdjkt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gbeqodkna.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gtdrzoxru.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fehbvm.com/Article/details/gewyvhbov.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/ggwxiiipp.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.zdbjq.cn/Article/details/grpkmnesp.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gpmlkaklv.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gxkpyhmbf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fehbvm.com/Article/details/gpjarpusm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gpilaxual.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gxysqqjdq.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/giotpfane.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gasplcgfo.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gjlohcmnp.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/ghleycchw.sHtML

[A20] 读取标准输入
来源：http://read.share.hesvh.cn/Article/details/ggxllrata.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/girqhkrcf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/gpltuqtwg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqcwwcb.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gxaovjjth.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/gntdcoogc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gkimkyaya.sHtML

Ruby: gets.chomp
来源：http://baike.hesvh.cn/Article/details/gyejtoahn.sHtML

C#:   Console.ReadLine();
来源：http://blog.zdbjq.cn/Article/details/golbkwbin.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gzxyjntob.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/giwaljrco.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/ggcpgstfz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/guancuzdd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gsiaxkpzh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/giigusynk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/grtpzknvz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gxqjreidj.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/geagcxcju.sHtML

[A22] 获取字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvsvctwmo.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/gdelfxkvy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/ghelooizc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gixhedsig.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/goqqtokik.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/glsnxnnlw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fehbvm.com/Article/details/gnndmsazy.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/giuurqcam.sHtML

C#:   s.Length
来源：http://www.share.zdbjq.cn/Article/details/gaspyjcoa.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqnatlnvv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/gytttlepz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/gzuttacwb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/goxyllnsg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gqscexeib.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gszvqlpzj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fehbvm.com/Article/details/gjfuwbnig.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gfmtpzcos.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.zdbjq.cn/Article/details/gdqklzzgd.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/gnynhnriu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gametxica.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/geoxqjbkr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gvrppdbaz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gxcssinyh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gngsshxzj.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gwfpmdzqx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/ggivcsdfk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gsvywyzgc.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gxbxdbfds.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gfoawydfz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gpvvenbuf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gseqbyoyr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gvutppplg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gbssyeczp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/glovzvbmk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/gfulwhhsg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gwvtctnon.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gmdzlqrvt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gonzynoeg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gpewycole.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gcrbwylcq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gyceopyps.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gwrbxmoul.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gdlizbpls.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/giibnoiae.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/giczdotrh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grdfxsabo.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gxffgercf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzcxbozyc.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gniehfdkj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gzjfduzdq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/glmcpmmgx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gjofadtfe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gpdtqcqxw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gyotfztzf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gxmlqeaol.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gbwdhcfmv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/grrjtjnfv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/girrwlzme.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gjqivrtio.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gzquqeljs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/giwrtbnas.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/ghvuyidfe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gwycqpsxw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmhlyrl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gewvwzvko.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gnwdcrcbx.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gwwptqcxb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/gfjyivxde.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gmrzbunhs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/glitxjrpv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/goowcstxl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/grunljdnv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gluuvyxcq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gxgfyqktc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gmpftbzdf.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gsskmdoom.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gmlcghdgl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/gctreokvb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gxpldmkyt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/ghvlxylvz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gdezjtdae.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gdfmxlvjf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/geynuwbqw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gcvvlxpry.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/grsyoucxd.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gocltusad.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/gaeyqvlsq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gryyyafwb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gesdysbwr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gddaofenx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gbphqhsya.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/gwqbjztbh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gzocwdlbn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gtynpdtmq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/goyfkrzbr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gdexdbena.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gxnpscobp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gzsribclc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gtgjyjcgq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gmbhcicyt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gdnbwnpry.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/ggtilmprr.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/guwcbwldd.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/goslpksgu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gqmxzufra.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gprpjepfe.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gmdpfjzpb.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/grtxlytlh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/giovmxhhm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gbiomtymx.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gyjkqqauc.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gspqbyrbx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gpokqzlzs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gucunazik.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gbapduedp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gtlwvjyic.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gofjydeyc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gudhdtiah.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gywfcaysk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gtkoiyzck.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gjmzklpdo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gsgptdwuv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gkwzubhcd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gtgxzemjl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gketgskbc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gedeyrcry.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gidzejiex.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/geyxifptg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gxvxduvqi.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gvmjprnjf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gjmhntprl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gcsoocnrq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/ghbepzssb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gvvqlnkfs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gxgywclbr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gzujnbhip.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/glwzewisw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/ghrnbheeh.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gztkyvqxm.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/ghlnbocog.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gyvccpkty.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/ggqhzgxdw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/ghtgdbstw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gcrjawhgh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gjgahuwjf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/glshiuetl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxnxwdtxu.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gtqlqavcq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/golsojtmh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gupxjabvx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gpmjkqetm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gvmqsmznm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gwaeignnc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gzshecmeg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/ghcjpxzmb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gircvybui.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gimyznmpu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gnfxaumjl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/ggylyfgxi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gsvenlmox.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gzrsupdrz.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/grvsxjdyt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gybnyofoz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gmtxtkusb.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gprfubknh.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/ggstjysoa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/glnjteaag.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gmgrigote.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/ggnjgalbg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gznkiknvn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gtxxiotse.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gtmcnxogp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gshdgjgct.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gnvdbxdcp.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gqnablyvn.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/ggbxcjvil.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/glpmoiali.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gellfinqm.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwgljgomc.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gfknnpavq.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/genchicur.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmowbokrc.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfpdrtuil.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gppexmhvp.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gqwbexogz.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gkgpakuvz.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gymsavmlr.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gskedmqkv.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ggnwsunam.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gmkdbukfh.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gblvpssdm.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gsutfqela.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggjgppxgj.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/grwchfhcx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giyyhqovc.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/galpallhq.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gldmjanpq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/giqtgcogy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghywydznn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gsxldwppm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gafsgyreq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gwnohqcyy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gjgklmbyz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvofpylof.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvlrukoot.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/glwyeyyjx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqcvjcilv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gejiojrlk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gvayudzdf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/giyydqrco.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gvvucknic.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/ghaqltkcu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gpdcbdnnc.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gayjobhld.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gognylkza.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gdbamurly.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/ggjepvaxb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/grxyaktbb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gdwwjjjfk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gnxhgezuu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gmcticzup.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gncvoeijx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/glgiicxyp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gpcrgdnuq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gidaayfex.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gqlwgjrrh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gctnncodm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gbkavfkck.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gvmqxgvpa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gmtnlpcsf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gcuflogzp.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gdvnxuyct.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gglybilxr.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gslqixvyh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/ggkxzmkcd.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gfmqiwgoq.sHtML


<!-- 参考信息 -->