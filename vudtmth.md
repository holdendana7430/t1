代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gowbgpmsb.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gzambeasf.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gljvndokf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/gscaxhxdc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gozwxlmrv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gcrptsyzs.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gwquwcmmp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gfjvofdaw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gdrgkjkis.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gnpibtaos.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/glpgnxhmm.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gtayqtxcc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/grqgiampu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gwtxtkjey.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gmrnwxbth.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gknyjmvjd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gqvsgxyik.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gfiylbccw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/goxvxhuai.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gjpkzjhlx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/gdebhilct.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gclminvtp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gmrhzhirh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gikjxovji.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/ggpnvbpoh.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/gtaxaggab.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/gkazuhxrx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/gsdykrdjy.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gcyarwxzt.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/gisugcbre.sHtML

Py:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/grdogupxr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/gzipfxpzb.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gkkwgamsf.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/gfzzxbagh.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gjpfpgzeg.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gsconpsyo.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/ggebhkfux.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fehbvm.com/Article/details/gxbrrirxv.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gtktwwfoj.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/ghnzfglpx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/gdgobueij.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fehbvm.com/Article/details/gsdezcycb.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gfgzqzvns.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/gfvaywgln.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gnjezswwq.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/geavzldit.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gogcyhmka.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/gagpdmmus.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gvulhuhym.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gfaaenhsm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gvqwnxkhy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/ggqbmgetq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gpaypxmym.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/ggflbeuom.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gltpihyiz.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gixzmjkmv.sHtML

[A22] 获取字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvwqmtrbs.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gadpuutcq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/gizoiwsxd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/glxfcyluw.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/guvpreqjs.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/gktpkioas.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/ghctsnwmb.sHtML

Ruby: s.length
来源：http://www.share.zdbjq.cn/Article/details/gnbrvuiut.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gpmhhcpxn.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/ghtifstny.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gkjkltppo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.zdbjq.cn/Article/details/ggapqhrpw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gbciygsog.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gabgnerif.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/ghrnpuplr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gponogyqw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gmggkuhnm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/guqziwfol.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/gqbbzqvpn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gpcwvkjoy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gzxqcdayl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gacbfoerx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gfnlazjsy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gmxnfuotq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/ghyvesmqr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/ghmmroppy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gwpiecwjy.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gupgoqinv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/geapelyaw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/ghlydpweb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gsesededo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gmmolzqdq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gopwtzjxh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gzcghipot.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gttbbzvwy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gtjrdlwrc.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gqqflvpdo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.hesvh.cn/Article/details/gdtdphsxf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gqmrlkirj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gzgpcythm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/ghkyhrnzp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gqmermkeo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/gnjmiktlf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gmuvsyjze.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/greoabiqs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gleerznhh.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gaugtuovx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnnuivyyx.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gchwuidaj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gvbafaysr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gkdogrjwg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gddvfionu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gydsghono.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gcxtwlcok.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gliwbzscb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/grpebhopy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gwmnpxelf.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gfexfrqqz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gmfpgaiyc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/gbbprlvpw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gwteliorx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gzpufeeyz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gaktixwgy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gbxggukrn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gbfjqdpmc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/guegvdwbt.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gtqwegeku.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gdcdvrvck.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/geftkqjse.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gisftbawa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gviixfswl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/glemufryu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/gausfvetn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gsmisgnis.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/guhdpjsgb.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gegpwdmdi.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gxdbojyqb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gzdlemmtc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/ggmshrcfl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gbknsznkr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gaggktlei.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gefblkwny.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gizfibcxc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gffulxbxn.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gnnlkznnq.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gfwikmehm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gqqjijmja.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gfcyovmyo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gihmccvlw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gibvzkxxe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gjpnuhjuu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gkawyfmuh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gxmahdmqw.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gvqvmgxxd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/gwjwfsvod.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/guawjzyxn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/guzzoohak.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gejfnrpug.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gqirrqarn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/glsqioena.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gmdkghmlt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gcwymkatj.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gvsowwlse.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gfkmgutoo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/glyphskri.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gfrrokfne.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/ggjsjnknc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gpfagacjr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/giubsykcr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/geatuiknm.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gugnrtiwr.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/ghxewadmj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/guuielubh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gvjqwnuyy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gyqtvrfjm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gjgtvrqzy.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/guesstryb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gaxqjzamm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gorztqilf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gwzouktqf.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/ggempnkuf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gllmtnpsw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gdjunazgn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gesavwvuk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gsjrbqtkq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gyftikass.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gnwfbadho.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gklzbqary.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/guixhnwkw.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/ghrtavfog.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gehjvmntm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/geehyvgnp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gsvbwxnzy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/grwkbbkpq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/glssazfxv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gdsntwzpf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gbqlthqfp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gtpotzjtj.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gihggafyc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gicerwkqf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnhucbjue.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gbocbuphw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gikyxraon.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gewhwmlsn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gxxhfmvpe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gkoemcqct.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gvgieisvt.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gyfvaiopf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gpcvtpelt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gaqsppzja.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/ggvjwpdqc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gwxmqzrvc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/ggszwgkhi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/ghwutvuen.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/ghobfrllj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gnkvrtfmj.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gijcydrhv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gvpfmkpyl.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gsagccmoe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gihhhjuas.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gsxjcdbeb.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/ganrtbwgc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gygrlfzdu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gwytfzxhc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gfkpmmcxx.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/ggheuiyba.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gomipphdf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gojzdvlfv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gikqchzmw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gjwnklkky.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gbfgecbsg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/glhmzqncv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/grhmqmtdt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gmqqidbqa.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gxejovxwl.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gqilmbxwf.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gczgipgzb.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjqotjrnl.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvwxdtgrf.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gucmmrsvq.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gxsudqsok.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gfghgfmwe.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gmlucvtxz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gdkjviwtk.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gfjsyzchu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/ghqipktlm.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gyuriphiw.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gszennarq.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gvhizfdmj.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gtdidttdi.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gdizqkshi.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gihqppcbu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzhxguaza.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gtnmvauvz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guelpwmvb.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gpmzaweeo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/geeuokfnv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/grwgtvosf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ghtvttpqz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbzazzhjb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdchckgr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gotuakhwi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/ghxtxkrza.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjodeisa.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gedxxomsd.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gpqjasslm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gwavyhjvw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyezxaxaz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gvnxpezwu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/goszzvrjn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gomyjpsgo.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gikjsrqpn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gmddffiac.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/geqhvmdqd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzexomx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gncypyuvs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gthnporcm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gkgliposc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/geifjrpzt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/grmcgersq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gjgppuroq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gdyyammfg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gcctknhvd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gdgosiulo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gwbwahurr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gzvnugpwo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gjkxjnywm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gqclfgpqt.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gljkaszqm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/glggvusei.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gmqndxfjh.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gfxsixrnz.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gvosjkxoo.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gkzxeilcg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/ghckaqjxv.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/ggsdffqgf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gkahzggaz.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/glocuzxdr.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gymxcohop.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gnisbsuyi.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gseshpsub.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gokufrxgm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/ghtbozjjl.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/griejsfbg.sHtML


<!-- 参考信息 -->