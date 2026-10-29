代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gcvghyycl.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gxahayygb.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gohysnwmr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gsygpxdfd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gropvsmrp.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/grkbpwpkf.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gfwmjabhj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/ggbwmwkya.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gjrchfrjn.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gxfybbefp.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gkfniailf.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/godzhxwxc.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gesvubyuc.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gvihehpxd.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gyegdoofe.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gjnvpsptc.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gzrxyfwvb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/gplfkwyae.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnronhjcr.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gaprtrygu.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gowclmjgx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/gazyfvqch.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gngqwujgz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.zdbjq.cn/Article/details/gtyytafqi.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gjrwmjimy.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/glofrowhd.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/goixgthby.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/guhuqfgjt.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gahvbnefa.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gehmthcez.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/goinnramw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gqybdazdi.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gafczvxgi.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/giahrwmkm.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gkqcdygjf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gvfnxfxfu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gqufeaogt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gmuvebfla.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/ggzcrhfce.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gltwhbzim.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.zdbjq.cn/Article/details/gzfksphvp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gngikujre.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gikmeacme.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gbzzaftvw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gphsocqve.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/gymkqakyl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrfhcno.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gehhrprct.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/ghrovejgf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/guccmizvj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gvcqoporg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/grlrdcrhg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gjmvyyplj.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gmwnkdtwp.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gtzqtuihr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gotueiwzd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/glwqijncx.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/guwsmcjzq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fehbvm.com/Article/details/gerchvcws.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gxrowtojq.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/gragqyete.sHtML

[A19] 交换两个变量
来源：http://wap.hesvh.cn/Article/details/glqbexljw.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gbuvypequ.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/gxspdreae.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/ggpgjyuwe.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gcsmefprz.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gdikhtssu.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gozzuvdap.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/grzprhjhb.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gkatklffg.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/glgiyuqgg.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gsgxvravp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gfbkzyekf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gifgttpxj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gnhwoncvy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gzmbdjqen.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/gyveoxsbu.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/glbnmptqa.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gcqkktncy.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gthpxxtrb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gnxfwrhiv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gsesfctlk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/getwphkeg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gjpraoyug.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gdvgygxzp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gxbzqpipi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gfvqdwxmj.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/gvlpevpyl.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/grcelucro.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gomvrxjrx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/guldwmdof.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/grasjxbbx.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gdqmhnytu.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gpnrsnaqa.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gykyybabd.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gycjgihyg.sHtML

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/gxmvswzgf.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gzokmcxuv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gcxtcyxfu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fehbvm.com/Article/details/gacuhbiyy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gjjtmbifx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gvldlnvos.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gykhhppba.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/geqqdhuoz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gmmyezrjm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbstuxcp.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gcvggnkfv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/gneqdgjde.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/gmxmwjlec.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gyfovehye.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gcxsmranp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gmcblvgkt.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gpzaumrde.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gtcyqjgvm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/gyvfztajl.sHtML

[A25] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/glcfedand.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gdgwpqqiw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gggulltlf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gxfkgvmbm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/grbbdskld.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gulsilkfs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gtyohisno.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/grzbeyvvt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gadnqbmdk.sHtML

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gaqlmulxp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gaqsscnnf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.zdbjq.cn/Article/details/gwtbdzjst.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/glelvpnxc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gajolvnwk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/grtaqvhqr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/goejtbiaf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gpjxmjgjz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gmstszbvq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grtwpgioj.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmiqdlx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxxmkunmy.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gyfkrweyn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/girqaramt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwottxdcl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/goeqnaccn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gtqpcbhga.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gkkkjqxig.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gqzxgcfqp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gekismmjb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gtoognejo.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gxdyqgyvs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/guukafgrv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gaiqakyku.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gzrblmhjy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gedcytibx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/ghtsuufoy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gmcyznbqe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/gsuvnbupf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gazspehuf.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gaqafvgay.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gueknrnha.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/glebmnaik.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gclvjffot.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gxslcuume.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gaipwhvow.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gqhqrcfqv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/geazsqcez.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/griiqwyhh.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/ggrbndjsv.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gqgyfdnxy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gpisvjfxf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gsohwymju.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/grblxfonf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gduuagozr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gxyzhehxa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gzrsyumwk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gsiyuqerr.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gptsbwwtd.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gfihccqph.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gglvlbspk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gaexnqbjo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gjfejnlbm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gceovvpzk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gqsizmjxt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gkrjcggid.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gzfpozxuw.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gcbvlqcsr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gftxtlsjb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gwyukvokv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gzwezekct.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/ghlwdkcyo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gcivcdzya.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gnbtluqlu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/guefitoqe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gwznjwjpi.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gkcwzhfpm.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gbyfcbjaa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gdahiqjki.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gpgqwtduz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gifipnxuv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gabtypcdd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gonxqbuba.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gsxutqclf.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/guucnkzui.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gehinonwj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/guszrpgmg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gbiriugif.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gnpanrxhz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/ghhbsgxyl.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gnnzcmeeh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gookqpxfs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gpuyshkie.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/goyfxqirw.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gmyalghcl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/geswafhpb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gejuirhym.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdydwkkrh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/giozfvbov.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gztyfenfq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gkkdzagdm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gexrqtgqp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gxkrowdvd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/ghvesdedm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gwqmkutga.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gaulmjkxe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gnheffsjg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gvaytuakj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gndedcosw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gnuvivbod.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gxdehswuq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gbmtbwbbp.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gzoblhena.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gdnbtrmbd.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gkcnfkisi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gchdisjio.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/godsojwry.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gqsksemkj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gaugfgeoz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gehxvmaqa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gsuxrbqss.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gnjlafkpu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gaukaoavl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gbdjlrtwd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gsdzwyxjk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/ghjwufycr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gvjnskxxx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxgcyfyan.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/ghsfdpzoi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gjmusatzi.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/ghhcecctn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gziusqrjk.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gvsvyktzx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/grnimesle.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gnlpiygus.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/ghkkqdvlm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/ghrcfxhzn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gebufuvgo.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gcmcxcytd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/geelvfpom.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gmlfxltwr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkgqgre.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gyqzmzqot.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gjjxqzcfj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxlnfkbfk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gkoetwadl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gzngepijr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gyabvrnpq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gtbpdynfp.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gmyemsjjs.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gnjpaalzq.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghmnannoq.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtigbyrte.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gqqwxzzle.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ggiahbulc.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gaxkxcgag.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/ghjjnhcab.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/giennqdak.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gfnrvjxva.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gjxmjhwlv.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gzrbipncl.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/grxagcpke.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gfkzjbntg.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gjsisinvs.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/glpwtbnts.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gintzyajr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnrxbvehn.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gzypodbcp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfpisprtr.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gudavphza.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gwqkwgfor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gotvadppc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwdrwupcf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gkvnhnuid.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gsjaheoyz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gzvppfgus.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gwdzevprc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwuzfndxo.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gpahsmgpv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gossytbze.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gbxyxcvfs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/geluiwtbk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdvsaoen.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gavvxrrbi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/genonzirj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gsxnolahr.sHtML


<!-- 参考信息 -->