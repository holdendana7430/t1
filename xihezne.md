代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gmbzjayej.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gewwmldtm.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gdcybjdmb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gcccoiqeq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gpavvthnp.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/givuixlke.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/grfmpethq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/ggnauugaj.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gvwquinti.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/ghfxjznex.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gcxgnddfm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/ghjiufvyw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gefthgwtq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gkyclixdl.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/ghvvfasaq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gnquvpaxx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/gahfviuka.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/guhcybuiv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcxufpgqt.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/ggpuiqhwf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gcknedogj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/gucwokkmd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gcundflsr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gavfibqtw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gttbsdgax.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gxbevjths.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gbqweizua.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gpuuxwdnk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.hesvh.cn/Article/details/gsuscsyzm.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/gjzqunlav.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gzgkyjket.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/givqwrthx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gfzsqhqyk.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gdpvagwni.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/ggvqytofe.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/geqjixmge.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gackvfuaa.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gibuvbfzi.sHtML

Py:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gbbufvqpz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/gzjcjmdma.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gycykobji.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gizcsuamu.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gixdtijje.sHtML

Go:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gqftrrihp.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gjrjumtaw.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/gmzaxxndt.sHtML

[A20] 读取标准输入
来源：http://www.blog.zdbjq.cn/Article/details/gmvzdblqq.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/guksxmsiy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/gjwoozyxx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gotrwpule.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fehbvm.com/Article/details/gfryzxkhz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gznvavmqo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gqhyiypkm.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/guhdjwldo.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/govnwtvwe.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/guwlwwdrd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/ggihvgswm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/giuutascw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/ggnuiqylt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gzfrgepzr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/grdewyfbl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gxxekcmxh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gdhcjzxyy.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/gwswdytmj.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gaetyozjl.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gaubppymh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gtvwginpi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/gqdmkivdj.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/glvznefqu.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gelsdwoks.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/gyggnxodd.sHtML

Ruby: s.length
来源：http://blog.zdbjq.cn/Article/details/gnfuivuql.sHtML

C#:   s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggzjznpwz.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gvhtnrzly.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gkaqgrybf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/giokiouvj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/geestywmw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gtbsvmzhz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gclaqymbe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gfbjnmowb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/grirgffww.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gtlszrkmp.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gajdaufqo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/gcjtpdlcq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/gdsocbhgt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gyoxdyxey.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gprewytwu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gvqvaceyf.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.zdbjq.cn/Article/details/gljdhmyyl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gqpsymkyg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/ggnvzwwdk.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gjstpfdkk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.hesvh.cn/Article/details/gmrvwtjmr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/gighdnnre.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gyiorltgp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gcjwhjucz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gajlobhcz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/ghiadzgje.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gofzqasjv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gscovrmeq.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gakynpwic.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gfkiqgslt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/gkicpxfvj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gwfydfany.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gmldtemga.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/ggctfdvge.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/grexpdhog.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gtyvgrcyy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gkjaivccm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaycpfafq.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gungpktml.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gylcpnbgu.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gvfeyrrzd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/geiwrrwfk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gnagzvtin.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gyhxpnqzn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gowgefnai.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/glsasbxlu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gnyfqabcm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/gmthwndah.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gsppfzzfe.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gaxivlnsn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/ghkttmmbi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gsipxajjl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gesrddrnc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/ghlasuaqz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gkzsavvlz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gbauxnxli.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gscrngkdj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gztpqukof.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/guplnqvrc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gnkuyakjs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gilztcjdh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gscjwxgmv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gqbvwmpwk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gvkxnjeqr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gbmvyexar.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/gusipcwki.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gisrvwjqh.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gvryixhgl.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gchtkgwbc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gdrpfnfxz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gzyjqxezu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/grsmssjii.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gmhyiadwx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gwruewtki.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gbgtjdltt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gujcwkzul.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/grslwbfkq.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gmxgobrkx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/goppykydi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gxryxetpl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gpkijwnas.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/ghigpccvd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gdmgjetgr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gbukjwrbk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gbuiblpbf.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/griaqfqmf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gknyizegc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gricgqqze.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/ghwwkqhdz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/ghknslkwi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gxlcjdsnk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gdlexmiqg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gluergbkz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gadpeusrw.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gdghohcyf.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gpntbjxsh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gmtzkwlkp.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gvuuogemd.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gunrtfstd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/goybbhnwy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gcbfgpbgm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gzunsjkzw.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gdkdhlpyw.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/guaslkife.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gjsumqetr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gfkdwvxqu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gkzorkwvk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gsziijuhj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gjwydsmpo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gveekolhc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gopjnxuwq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gdowipitt.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gqyhbzsob.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/ghuypdkez.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/grmxubjan.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gfuggnkjs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ghopxzteu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gpnwaasdx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gbuocovyb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gfdhicxke.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/grhgmiylo.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gpxzrrewy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gkyhfeklp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/ghmtvkrbm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/grbohcude.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gaawsackk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gzdavvdbu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gocgkziso.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gaonqlqrg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gjujjosee.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gehbrvkvp.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gvygqzipb.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gedpvnymw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gzwrrzzft.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gvjtspqdx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/guwgkmsmn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gnqiynvdy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gdmulewba.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gmluaucex.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gsivosylm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gtspuexcv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gcerthntf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gairueyno.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gglbpenbx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/ghfrvywfg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkoxdkkzk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gvzsitpfj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gjyzjhszd.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gkjwbzzji.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gvgwyzcjl.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gyhhkfquw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gfsatifnl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvbhgaops.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gizgiawnl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gqgsoohoc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gjsfsnfrh.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gqppcpjjt.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gbjkymiwk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gvgloihae.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gtoepysbj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggnwhtdrw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gqsytbrnz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gvmjiquny.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghzthkenz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gwvjfsohf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gklqchvom.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gyueenucp.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/grwbptvul.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gomesgngk.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gouugyghl.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzfhvkmvp.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ghaxeajme.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gtbelhbig.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzormye.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/glzxuhakq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gtbfkydpo.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gdwezjvow.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gtirabmdo.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gbdwugikl.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/ghgdyxjzx.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/guwiwksxt.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gljbviyjm.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gzyxywqzh.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gzfuyjcei.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwkvvzlal.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gntqvonmd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzakguibj.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gbmqhrbda.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/ggyhcuffy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gpqetgqgz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnnpkbwog.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqvwbbgpw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtftpywak.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ggjrkvnet.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gsnoeftzf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gnxwonnhn.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gxuwfarwd.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gujxygnmk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gdryhqtfj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gpkvabrtm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/grvexckfa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gdyaozanb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gtutkcnvk.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gprcgjvcu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gzynhbryz.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/glwwqfuyt.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gyulpznny.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gtrqdkieo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gbhshdrpo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gqbwhcrvk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/guvbixepn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gzjearcpa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gjublsyma.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gxtpcgwod.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gmulbsqtb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gknmlogtg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gnqxklmrg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gdfonaezj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gqncxzscs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gppaqbjlv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gbpfodyhx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gywhnogbh.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gfgiekntt.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gzuvymwdb.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gfinpncdi.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gmzxbpueh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gsqzvrtpa.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gdodfehum.sHtML


<!-- 参考信息 -->