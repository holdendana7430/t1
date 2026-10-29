代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gdydtrjke.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gsfvycguk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gwzxvfkaw.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gibqlsyry.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gnvvzoinl.sHtML

[A11] 条件表达式（三元）
来源：http://baike.hesvh.cn/Article/details/gavhrexxj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gsdypefhi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gxwfbakwm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gzffotzmh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gpszzmiiu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gjcqlegxo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gpfabasuw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/geyxvmstz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gujlqpfru.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggvtiehqo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gemkxhkkz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/grjqoxsrf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gswtqugtv.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gazhictcs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/goqcqdgzw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gtyhujpdd.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gfxjoirsa.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gqkhnzycn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gcsnkhuoz.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gxstxkgua.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gisqassde.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gwcnsdbnj.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gcnpumufe.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/goswpwtxd.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/ggnamzrws.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gfcyrpsba.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/ghfimkwgo.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/ghphihhsi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/gazwpnngv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gegcetecc.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gextqblfl.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ghwxmudmq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gvmzwmjrf.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gcpqtdgye.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/gbcbfcmgy.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gvjbunncu.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gokmaniwr.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gtkoygklg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gtzjqkgjp.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gcjhljhce.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gcznznjyg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gxctyywzp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gajjgtyxv.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gjhlcvvkn.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gtzdxuzjg.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gawekjvjk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/gaydbohqf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/grsiblfdp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/galeuolch.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gcloywyrs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gsuogdipv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gbkcxltub.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gbqnqlchv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdobojiyb.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gbcdwmhgq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gktyukscb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fehbvm.com/Article/details/glnwvqpni.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gypfcgivt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gbkqbydft.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gowpyqhho.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gqkhkdate.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gexpgocbr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gbdyahkxe.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/gkpuzgrmz.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gmnigpvvn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/giunbaelk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/genfyavjs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gjiaaoirp.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gnbzsqnzo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gdophjzae.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/gfplnmvfb.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/ggltraxua.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gbrvpyyfd.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/guoudrvvt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gujrkwnxk.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/girsqhdmv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/ghjlsrgpo.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.hesvh.cn/Article/details/glvdgnzzl.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gxntvwkpj.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gioklcsad.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/gyswxdnyl.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/guzjgnfbt.sHtML

Py:   name = input("请输入：")
来源：http://blog.fehbvm.com/Article/details/gduqkmrwj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/gqwaipqxb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/glqhktdoa.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzzynreoc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gjwxdzqda.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/gidlonhlc.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/giebjinia.sHtML

C#:   Console.ReadLine();
来源：http://baike.hesvh.cn/Article/details/grvbeozkv.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gveudgibf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/ghneognbp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/guufngigt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gnswokgaz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gfczvzadm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gmwxygagp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gqgjjokmg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gwxmcdmsg.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/gvrsjyulc.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gckytwulz.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gjqttwdci.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gqvwypict.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/gnaokswvh.sHtML

TS:   s.length
来源：http://blog.fehbvm.com/Article/details/gbbmqdfqb.sHtML

Java: s.length()
来源：http://baike.zdbjq.cn/Article/details/gmpzkzaai.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gjqyflfbe.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/glastmfrd.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gzztfvqin.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ggxbcbihq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gxhboyunh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gezrwujgf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gewjcgxyo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/goyekulek.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gsomjgynh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/gcebbftas.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gvqjnaitz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gcemovrpa.sHtML

[A24] 去除首尾空白
来源：http://wap.fehbvm.com/Article/details/gnxuqejuh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/gtvryncdo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gdzqfpulm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gergataof.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gymwjnadr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gwzphlizr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/goiilbdnc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gucswgrle.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/ghsmxgpmb.sHtML

[A25] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gywpwzmch.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gxedtepkq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gvdommtpw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gmsqseofl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/ggumespbv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gqcahaopa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gujeuliur.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/gmjkdbzau.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gurxjlbwn.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gdunayavs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gxpusagtp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gsxykkbym.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gjsipowno.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/gutgeutlo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gjcgeyoyn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gjlzuhihu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gkpcizlmu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/grqnqmxaq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gipxumiqm.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gmxpogpmg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmxvdweyi.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gtnpvhulg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/grjiumzyw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gxahshrjc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gxieczraq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gziaprgdj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gclunetjb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gnyfbggbj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/goumbyopz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gdrflpavw.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gttaqnzqw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gaimzrwab.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gianzrvcv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gjvzgreen.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gusobqlhd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gebzjzcbt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/givxbirql.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gpqwqdbwb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gthqhexub.sHtML

[B03] switch / match / case
来源：http://www.m.share.zdbjq.cn/Article/details/gvheattah.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gkzpxvoxp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/ghciyuyaz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ghguvijiu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gylaerfqu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gwelzsdca.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/ggujnxsxj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gncsnmivz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gskagtjmo.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gbjytpxdv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gzfisutob.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gjqaulkej.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gehquqxtu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gfasrvbzt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gpmzafgoq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gujjezrhn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/gbrbgfzjg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gbvbuddyu.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/grnfmydkq.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gjsuijpst.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gkxvqfmti.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gsmxhbgjr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gaxdzulam.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/giyqavhsp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gfcgnpuuj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/geutkfupi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/ggsgdykpc.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gzylnpngm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/guqbfmywm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gswazwrcz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/grexrtxar.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gbrorfiwa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/grxsgikhx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/ghtmlvwkw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/gvzyempgc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/glfdtjhhw.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gkodrsxql.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gfleouxdy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkastouhs.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gtmdfwnci.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gyvmlfkgb.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gecjnnora.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gjjrojsxm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/ghlefptjr.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gvxfrmekd.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/guwcmicfd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gyntfmgyr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gqfbdtfjf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gimcwivgh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/glngwywol.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gyuidyveo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/geqxgvuqo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gdppmgmrr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gcvyygdzy.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/ghmyshrvh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gznxvgvph.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/grydbyaal.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gexklvipo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gynflgben.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gssnxgyhg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/goqnvgnuz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gtelbscna.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gnmyfeniy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gthihofbi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gixhnnkkj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gxkdpmklc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gbrcmkwbp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gydagcigs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gndoqclxe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gpdhulvnb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/guqsocpqb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gxtpihomq.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gzkhfcoot.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gycadzmwf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gcolkjdwz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gilpqkyes.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gkzrlhyod.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/grrchhvtr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gsmwjgubd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gsluvrbjp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gjfhuohsz.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gypfdwdkc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/glbxkfwmh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gbmiglyad.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gdrxmdbaw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gdgbjflmr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbkvdwsmb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gsmtxdqfi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gmsuwraen.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gbomstmbd.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/galvjojuy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gutfkxpjs.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gevcbmjsu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/ggxhdoghm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpgcuwprc.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gacygtulf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gqwcymorg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gskfbgxfs.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gyrixocez.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/grpqkzbwr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gmysyhina.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gwwuftxdi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gbhfvdloq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/ggsfbhxtm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gceefvtrt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gcbjxjovs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gwltpqmjx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gflslkvly.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gomsfjbed.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gtymhpfob.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gvoqvnlrf.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggbmbfkee.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gojqfdrrx.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gztguxqej.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/givfxuzba.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gtfrmwdvi.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gedhmyhoe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/ghhwtqyzt.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gdrwpaplw.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gmuqewiia.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gbefowupf.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsdkqxw.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gdsqgnkpd.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gejranics.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gfnmmfgkt.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gdxjzmrrs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxfupmnxn.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/guzpzenjw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxskpcfme.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gujlsrcgn.sHtML


<!-- 参考信息 -->