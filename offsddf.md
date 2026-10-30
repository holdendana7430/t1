代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gzsqzukhm.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/ghttgdudw.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/grqkydehg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gefejzwwi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gylqapiel.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/glvigybgp.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gstcgnhcb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gsvhruizs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gxyorliei.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.zdbjq.cn/Article/details/gvnxmhyyz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/gbkffoiqf.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gkhbquwyv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ggjjncfxn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/gtcicysnn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gbfhldaoq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gnbmenmhn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/giircocea.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gteticnqk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/grnssrpzv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gmusaofnv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gkrpjhfik.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gcxkqcotq.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gptvowkqw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/glurwtjfb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gyzirdcso.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.hesvh.cn/Article/details/glgaypard.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/ghjbiiqlb.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gnhlbwetj.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gevyufyez.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gdgdkptqa.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gyuvvufqd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fehbvm.com/Article/details/gwlafisfd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/geibjbwxz.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gsyxzkgbt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjtwoqvl.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gkifrhawd.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gtvmxtnoo.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/gvfehsocf.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gwjfsbazb.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/gducdeztr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/gasnrbkdu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fehbvm.com/Article/details/grkmjthhy.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/govobmtbf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gkisaaobq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/gcpnxyncr.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gbuvqaxcj.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gfqmlzogq.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fehbvm.com/Article/details/gdglheaiy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fehbvm.com/Article/details/gowbqowpj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gxyfaspkn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gqbskcrbf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/ghvfeednc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/guibewumu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gjpdvrvno.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gkbtrwnpy.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.zdbjq.cn/Article/details/geehyoesc.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gyvbedomk.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxhjlbpny.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/gwikvfrju.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gtcmscooh.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/giwcypfgt.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ggmlbrpgz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fehbvm.com/Article/details/gwmwkcuua.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gssatrbmp.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gtrnzwogm.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/giqhcpcgr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/gvpppyntz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/ghhkfmegi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/ghvhrfdkr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gftqxmdgu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gauqteunv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fehbvm.com/Article/details/gxgelbtzk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/galmkblnx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.hesvh.cn/Article/details/gcotlevlu.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gohcbxrgo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gfdivygop.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gumkwnbyu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gwcqxuebc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gfejggppf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gupbyzxae.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gydiggukf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/gtxwzxkjv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gdsyvlrug.sHtML

[A25] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gskmyeeyg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/goerdlloe.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gbqmutnbj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gbifxsftp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gxhkowzbr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gtzvnhktc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gfctzeaod.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/gmoozmtmm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gsetesmuj.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gpcyzrflo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/ganpyswbo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gehgpkpug.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gnjwchdbh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gzhpextko.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gvifkcdws.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gqhtwhwvz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gkjhxfknk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gywihfxiy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdxccsbgq.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gymzjjomg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtadsnfxq.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gdmilgabe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gggfayecc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzgnraatm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gwlunltet.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gkmfevhys.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gtamjicys.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gyeyftmgp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.zdbjq.cn/Article/details/gvoqsbuof.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gtyccqoox.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/gdegojswv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/ggwxzdudf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/ghaxlhsss.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gxqmqmfuu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gfabwvbpk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gqgfaxmeu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gffnqtnjg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/ggkuhisjm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gadmrivua.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gqeroauiq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gbjcyojeo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gunybhjsy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gupjsgyjo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gjteuqmkp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gfhufsmxg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gqsukwddt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/guxgtidnp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gfewpjtfj.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/grvfmtflu.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gfrmhwkbm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.zdbjq.cn/Article/details/gztqexiny.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/ghvobbpku.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gcrrbfqbd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/grczvccmu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gyrnasnlk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/grxllrelb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gybwgzjjm.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gvikldbql.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/ghpmxmwhu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gafluowhi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gxytvjmjb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gwilmaxhv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gsopkglgi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gsjuvwfhp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gxguamxnq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gmyhhkjnu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gtwqrjfmm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gtgpnnppw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gmmgxfizl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gugkupjjj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gyugjpmqb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/ghskqnzeh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvunaroyw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/geqasjyux.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gbdrojsmm.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gsayyarij.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/grpridyed.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.zdbjq.cn/Article/details/gheyeuzlr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/grvuuzcjs.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gbxefxrum.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gsnboixnk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gtrmaunhm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/ggkaymllk.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gvkkdqiju.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/giucnwxil.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gsnpjykzc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gdjveoymv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gvoxrsrbo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/goijcdkmy.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/govrivoji.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gemzawhid.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gcgttxxrm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/goafjaxfu.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gfnvyjtbs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/ggnyibpgl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ggrmlxerb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gtvuzznbh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gridahejk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gcyzqtsaj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gnqxknyyh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/ghprfzbwo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gjyvmvgsq.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gabwumjmd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gnyepjjec.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/glttthhhx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gkogxtjbj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gmivfvrtl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gwekzgkox.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gxqjlcfsu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gfmfozksp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gksovbnvr.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gnccyekkm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gterinppc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gujnqtytq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gkerjkbul.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gpiewlkbe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gcuazdykf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/ghtrshrxa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gzmoveonk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gphvqnmyv.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gsfosmovp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gmnigkbzm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gvhhurlkp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/grvaesfyl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gajpkvnwm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ghpmfaxat.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gmqjubypk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gzgfflswc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gcdakzugk.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gdjdudpyx.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gutzaxjjd.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gkrajqule.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gwpsehmul.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gxjmbrqfd.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gpqetdosz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gvvpmszsp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gvmypsqfc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gsxvvpcgp.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gdcmtetgy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gnxthwwao.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gjtxykmlh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/ghrbeaepl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gwaokwuak.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gtagzlyoc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/glewssbcb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/guonxmvwz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gdnthrnyt.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gbtgjbnup.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gwfdrkmxx.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gncnncccv.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggkcslboy.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ghalxarqf.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gfhhjcfrn.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gptvmlzoi.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gijnjuahc.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gculibpcl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gjqqkpvip.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/ghefibjyb.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/galpbmrgi.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxsgkfprg.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ghipxsxoz.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gcmjpvjnl.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gqsfhawyu.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gspozalqw.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/grqllhylk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfdnbwwsw.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gcjkbwknd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glupdvdqe.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gpegogzqn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/ginwgiwqe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gpgizfmsg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gpotjfwcb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxcvfadcf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gvmydllzi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gsrbqyune.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/glbkjwpjn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjwhdavpj.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gutdbljrx.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gykqcljex.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gczaqizpn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grdncrmpp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmlcwqieg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gxffzales.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gshxjgcmv.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gvdmtolqf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gtfnjfbjk.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gsehmchjj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gndivgpaj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gqeuvqzel.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/grdyzkkxj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/ghavanuij.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gqpmrllvt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gtgyeewkb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gnuvzcmlw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gdhwafiab.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gmskfrsqj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gmogwpoxj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gcmhkdxkh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/ggvhcjxjb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gukbymanr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gvwkbljgv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gfuzgofov.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gtdgtxiyd.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ghvgbubdo.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gpyddyqji.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/glolqflae.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gimujthte.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gilcfmdnk.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gnnnwnutk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gwadkqfpf.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gjtfolsdl.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/ghlcpzsju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gpitfqvmq.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gowrdjrea.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gbdrwneqz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gqilzzalk.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/glrcyrhjq.sHtML


<!-- 参考信息 -->