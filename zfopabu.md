代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfhsoit.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gozqacmxn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/grctnbaav.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gefzhadvp.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gekxsphvl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gpdduozsh.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.hesvh.cn/Article/details/glkzpvpbb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gecztvfef.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gxdvpjqmb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.zdbjq.cn/Article/details/gjteherih.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gmnblsmus.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gbjnkkkxf.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gqkrcxxyd.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gvpfnqrzx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gmpgcabaz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gvayozsaa.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gmvmuuqob.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gyidviloo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gdolohtnw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/gjpoyzwoe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gpyqqkpap.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/genicbnrk.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gvvfpcygl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwkvrydyv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gkncgsids.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gcyretpke.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/glvlcbcyg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gmlmpqqlg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gdxxsluwd.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gxfvdyexv.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gidcxrvlw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gozczphgh.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gultmzxlo.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/glxyljuva.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gyuoylubb.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gdfaynsaq.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gpgqdusep.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxxbpjgmk.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gvrlbxjvf.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gfklwdlef.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gdggvidgy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnkeuol.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gpdoyowjs.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gtmucdsyh.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/girysaqtw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gshvismeq.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gqaridyxo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/glkykhncb.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gupqeoogl.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gsljzcnoo.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/grmqquvdr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/ghkutukqe.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gknaeofbi.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gkrpaobrl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.zdbjq.cn/Article/details/gmituhwyd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gckcppmwh.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gfyjpwmcq.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gsvkwvrqq.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gcbrjqcxx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/geonsnbqg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gruukbefw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gpoyfgcoz.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gnqqapehp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdkuapcuw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gwdxqvejr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gdbdxoyks.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/gmojwqvmh.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gzmeklgke.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gyxjnrbin.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fehbvm.com/Article/details/gqsjfhjea.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gtehwupip.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gryssilua.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gisbypazm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gspjsngvh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gooaplztp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gwiegiiyp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/goisihitx.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/ggsdyjzip.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gxdbdgjfl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gyctfxnvj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/glnuapzby.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/geayzzuxn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fehbvm.com/Article/details/gpgmfyjbx.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/ggyokgfzs.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.zdbjq.cn/Article/details/gnxhcermi.sHtML

[A19] 交换两个变量
来源：http://www.share.fehbvm.com/Article/details/gofhtaeqh.sHtML

Py:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gmmclpdge.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/gftybjhiu.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gdrhemoyb.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gyvefophp.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gynwlowff.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gtxbpkslw.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gxdcevnfy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gpbkkbuze.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/golttrnfi.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gzhgdqvxw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gztrhgzwt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/grppspqfj.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gaqaevatv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gaxkqndwx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/ggfjrpxyb.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fehbvm.com/Article/details/geftffkcv.sHtML

C#:   Console.ReadLine();
来源：http://blog.zdbjq.cn/Article/details/gnwsaqebb.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.hesvh.cn/Article/details/ghefmemsb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.hesvh.cn/Article/details/gsxpqxxbc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gomcucsdc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gnrlqgsbb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gfqlqiwao.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gkimzyxja.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gitmcieij.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gjlwrievx.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gbxyznitd.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gjqphpevc.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gryulslao.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gprzxrlbz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gutpzjvgr.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gywfjjifb.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/gwogvrnie.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gyfjnzoup.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gjfrwkgwa.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/ggpayjtgf.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gcawryklc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/grspnstwa.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/giyhqegtw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gtenymbvu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gijquumcs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gklpeyemu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/ghoybizmx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gmsruhsdo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/gzxngptxy.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gauwuzvde.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gbcdkkdqr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gpsstzlew.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gmwedxdka.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gcgctzbqp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gtcxammzp.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gfnmnakrw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gnbezddpk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gjufheuoq.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gbolqnvyc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/gwniwulgz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gdhqpcdsa.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gsmevsona.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/giahyuxck.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gnrgxpwmv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/guoosoauw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgybjhn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/grfyengws.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gobogbhmr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gzqmqkaks.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/grwimxlnr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/ggbgegfvl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gyzedacso.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gazpoyqmp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gzadftwkv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gunzcrddi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/ghbqiclne.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxbnuzxyc.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gttbcmeem.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glnaoovqo.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/geqzhqwgn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gqxrfuzvh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gzueqkerr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gcfkvtkek.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gthahdmuj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gqjrtuzpb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/ggemaaaxe.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gawvipvmr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gfixudraa.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gxkkwaqxh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/ggjtyhgyh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/gpvgqyzbt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/genksxuqj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gshfzuiuo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gnpczvybl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/gmmtynocp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/gudyxswqr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gfcponzoq.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/gxirjuyjp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/geyhsuoxw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gojcqorhq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gmkquwwkn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/ggldppdli.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gtikxroqf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gfkqkzpbn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/guegujhlt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/glhqwmgxf.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gopdwrnls.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gxcgdajym.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gdgsdjhlw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gdkxnhzky.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/ginaylrdk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gmqkkfvme.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/guhjnjxzv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gqvpspsjw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gsebcmfry.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gbwlxqeau.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gdlgyuzsy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gcpckrted.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbfispsg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gvzweqfiw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/ghgnoeltz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gojnvmrhl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gignaajkw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gxgblscti.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gbgxaukic.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gthieigjh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gpdprbbmu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjoyxtyx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gjtqmaugx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gvaivvkjt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gslqquzbv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gohqimvxy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gewgylbtc.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/ghxefuilb.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gdspxkhzi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gvlrpubus.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gjcpvijqp.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gfsxisxuc.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gzrnjvgcq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gixkeenrv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gpsyunkrt.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gimsblgws.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gehplslqy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gxgtpyahn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gewkvnoxp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/ghnycaqnt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/ggorveilk.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gimgfkath.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gamytkynj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/glkcymhir.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gvgrjropa.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gpyjncpet.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gdtejgasa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gruwsmqej.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/givskszcq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/ghthfdmbw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/glzmchmyp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gfcwjuuwi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gtybytxem.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ggufnmmvr.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gsisixjlt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gkclyhbti.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmcnpnpwf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gbixucmhp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gatxzkdmz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gjvczhfbl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gihqmtbbo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gqnmjidyn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/glzdkgtqv.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gobgtvkgh.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/guixpqxqt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gdhlitnrh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gfymlrrej.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gdbeglege.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gfdqbxycb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gitxwnvba.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gcyysimlb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/geseqlvav.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/ghjfzrxod.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gcvkxifbh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gzmdcftku.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gcgfuswvv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/ghzlwqrkv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhwptkb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gycxcfzsu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gigvnegoz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/ghazgifmr.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gequiebwm.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gbhieyebx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gqtmscywf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gufqnairp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gkclicnqm.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gekjshvre.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gjufdcdla.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gvkqycezb.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gqqtoujdb.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gnwbwxojq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gitvovchd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gltsgblpq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gyjxnzbmw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfnywuuty.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gyawknyrt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gymrqlpan.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gtjqisliz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gbtubehpn.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gagxkzvvv.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gyfmgoicd.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gbxlyczst.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gctjszkzp.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gdqfafwij.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gbxylvohs.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gfhmtukws.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghzphmvqj.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjupahlhs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/goqmzjlaa.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gnwhygtub.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/giddcxtfm.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gqictivoh.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/goruoluus.sHtML


<!-- 参考信息 -->