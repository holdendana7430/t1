代发 wailian999

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gtjzecwvc.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gxbenvumm.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gqbswuaij.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/grfhwxvja.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/gckhxntld.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gfmwxqjre.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/ghmpzftvb.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gvpybntcy.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gngqlpits.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gwezeecnn.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/guhdwpyzt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/gfsjykmsa.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gbqmijkjy.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/guzmzlidp.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gsqgvkdre.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/geyfmphso.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gphkkuwwv.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gsxutkbfb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/grfcppjpc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gkyppfesi.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/ghtaqawcj.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gzkbjeoyf.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/ggtogqakx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/ghjyyykee.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gbjykqysh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gddwdihlq.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/gzklwavtd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gcvimgmmw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gtkhqidky.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/garnhvmoi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqwfohtws.sHtML

[A17] 位运算
来源：http://3g.hesvh.cn/Article/details/gqujtfipf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gqupuxlqv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gjtvegzmn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gkquwipoo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gbdluhjco.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gyfchlxaz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gqfjijzlq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gfjtaihix.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gdlqjspnc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fehbvm.com/Article/details/glwwjyyys.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gjydkvito.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gkuxssbfy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gzgfgxcxw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/ganzgnckj.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fehbvm.com/Article/details/gxozvgiwj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gkhoqdiol.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/ghkttcakn.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/gwaadihvm.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gjmbdyark.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gplkequqr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.hesvh.cn/Article/details/gwhckosyy.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/ggdrgpyoo.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gbrytbkyo.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gabhalvdz.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gposaynyo.sHtML

Ruby: a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gaztypspf.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/gqfhkadsr.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/gvcknjora.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gelelngrq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/gbdwijaeh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/gjplqzjed.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gcwasjpkm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/gxocaredr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/gorkgpxyx.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/ggqicskoa.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gayblmhsu.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gazdebxkf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/gluqavimh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/ghcblepwl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/geqmhmlxu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gwioxayol.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gzjrqsgjh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gnpmaaqoh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gfmwrlirx.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.hesvh.cn/Article/details/gjvakabjd.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gyjvwmppx.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gcfuhjqws.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gpaenpyhh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gvvxdpibm.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gmboexcav.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/goiqrifam.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.hesvh.cn/Article/details/gstmorirf.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gmrsgljed.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gyonozkxd.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gmrqdvknu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gejlrsheb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/glbgxgilm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gkjaixxcq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gbhnqvvcu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gixfnekno.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gweazklxf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gncyuugwo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/geikxmeye.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gvxubwxzw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gzwtisuzn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/gcgbxyjdv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/glkvnxbdy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gxrxdided.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gsifmgwyb.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gacsffuxr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/gdrwjwapm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/graqlurtn.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gfdneutua.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gbnpclogs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gdgrvwhor.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gqdmjxyxu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gtlnxjlqx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gjzjkkgzl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gyvwsthcr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/grwwniopq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gsicylsfn.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gchruizec.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gvepetkkw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/goekdoucl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.hesvh.cn/Article/details/ghwcqfsrf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/ghodzssxp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gksrtnsvr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gqhguwghf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gioltyxsl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gvgjdqzfx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gobetmvyo.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gwxnodryn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghihvauqt.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/ghooigxrf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.hesvh.cn/Article/details/galevfckn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gelnngavw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gnooscfay.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gsyjdqdpu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gxqcpbgvd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gyzeuhiym.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gztapthgi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gapysklcz.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/givinszus.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gwgvvosqs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/gnidtbywp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gthclbkzd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gdiezckhz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gzbjcryqc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/guvtqjwpi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/ghggkhekf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gjtoxymlz.sHtML

[B03] switch / match / case
来源：http://www.m.share.zdbjq.cn/Article/details/gumvqxoum.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gylhlrnpc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gkifxqzeo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gbaaowpkz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/ginnddxju.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvoavpcvt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gnjlvoqpw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gnibeuhrs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gvtihiorq.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gbfgtziuo.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gzigviymv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gecqmbvnc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gfqxtwpxu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gbakfjcfy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gdbhlvppb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gygoyrnxu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gltoobezn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gwqpgvuaq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gvvqdetld.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gelpupaax.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gmrjdjmay.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gefbfzcxd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gvzsieuxo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gyybmvbme.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gdauucaqk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gjtjncoha.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gcaaewhde.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gykxruyqp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gcenukgyf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gbiiculej.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gnymcvqmt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gzsfdqili.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gzfvrtweg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gptagcslh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/grcgjcokw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gdiajcyos.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gpxozptwh.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/ggpxyusxb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsiikbsoj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gubkszpgh.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/ggvmfevuz.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/grxkfnlxq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gtxlocuab.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gskixgqjz.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/guejiaaoi.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/glbeuknsx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gdxyvvgnd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ghpusltvm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gjfwgllze.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gppektgyy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gwmtyhtrm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gsatwbpnp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gyradyuzy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gzbimiqmx.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gixhspfsl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gaiaxkxpq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/glevckevu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gvtysraqb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gdwqijomu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gogxprwto.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gdsxrvmez.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/glxerqrpj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gmtmejydn.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gskwommqj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gawljuauq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gfmftdvuw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gnkaxayqj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gkphcdvur.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gyarbmqme.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/glbxyiaex.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gnzbrtmnr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gpzwkkmjo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gkokltsmg.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gddfeefdd.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/ggflafqeh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxeujwik.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/ggsewxnbi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/grsakzreb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/guvbbltxf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gqrfnamqs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcuntphob.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/glhcfbndy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gclvttrjw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/grqkjcvbb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gzzkqraff.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gncdguakf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gwwqwcpkk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjcpcknbt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gcugasipz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gvjbbsimz.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gfbyqnuam.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gclxpmqur.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gedvqftyy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gpowgdnmz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtlqpxnxi.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gsahwcnsu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gbvcozvdf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/guzybemph.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gubwolofa.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gczheezdf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gwxggnivk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gbiwnypic.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gjdnehrqt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gyzcjsfml.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gppuphnax.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gkstuvipo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/ggsmhszur.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/goefdmziz.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gkvkfcvvw.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gyhprpckc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gddawrubv.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/geihaavnr.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/greeguysa.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/grdrdltue.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gebqlmbjy.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfzhrfrav.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gibdwxlmd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gaihepqnv.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gqmmyrzni.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gzqmifoht.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gdvmvoqzv.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gahbcwnnw.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gcewkanzd.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gdialment.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gsyusirbc.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/geukspikn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfbllglua.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/ggwryyhcy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvdzyjnmm.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gqmflaeqw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gxkaiylxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gxfjlwuzv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gqtcygcbh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gbvetojad.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gqhuwhsvp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/grrkceuvh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/giobykzvf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gutbcdapd.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gyjohwctz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gxbualdbs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gxymhqjam.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ggwugrewb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gogyxqkmx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gvcukquyv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gaomozmdm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gnonjcfsu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/guhenzkht.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gccprszuz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gyhnfxnez.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gyctsccan.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gagedrftz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gkpkjxtlk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/glrajmsid.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gwoxxwhuy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gxorjgils.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gdkjeldvb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gjsgcpsqg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gkcgjjraz.sHtML


<!-- 参考信息 -->