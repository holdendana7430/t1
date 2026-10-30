代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gfvvnlbrq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gosjeoyoe.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gpvwvzwzg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gmpdsngav.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gzqhfaxjo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gnxyahkap.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gpqlaipnl.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gtmoqraar.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/guikeknyw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkuhblxox.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gduqtnzqr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gohvjikgz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gzceunhic.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/gwpswkoer.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gamhwmjpt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gpnohuprg.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gwbeswwom.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gzejhwkkz.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gdnbhmztw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/ghvfiduou.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ggfzmkqft.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gvyavoesa.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gnovjhevn.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/grpztwdbu.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gqtnzmyqg.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gtpxkiegl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/guvjnwoid.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gazbppodk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gjycoafko.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gmunxinrd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gbbwjafug.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gikrkdozj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gzwllxprz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gvsgefjhf.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gotkvject.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/ghdqcofhk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gcbrczkoi.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gnzchesiz.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gmprqzznr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gxkcwcqcz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gwhbjrvqw.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gnhwrlzpn.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gxupzwedp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gyosjgveq.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gpvhgxhvo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ggvmgxbxj.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ghdgtoewi.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gpndbxtqu.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/goyzvypcx.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gnuonljsb.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gdfbhdsma.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gwxypxhsi.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/galwtklti.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/ghwafelwx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gxwpdjghv.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gosgnywpu.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/ggnnbkvcd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/gkrfxzcbj.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gcoarfyud.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/gsxiyhvvk.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gtlxtpaqa.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gyebtjdkc.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gtfuwjzvu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gqyrbkfbi.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gdjzzfbxv.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gynycrbyq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gtgulrvvq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.hesvh.cn/Article/details/gznittvop.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/gebgbaesu.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gzuzxwqin.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/ghopbyupf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gfaoqzxkf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/gvythtvvc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gwizggacm.sHtML

TS:   if (!x) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnfcvdlur.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.zdbjq.cn/Article/details/gbbyctffo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/ggtpgamuk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gqqjvphez.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/gxtfszrgl.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gcxstqnba.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gsitabonl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/gazeffkux.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gmztlutlm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gbcpkvvto.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gnqthsopf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/galpdfjgt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gxlcmasya.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gjtafvwep.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gzygbgaqx.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gleaymhgs.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gkpfrjoul.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gqcrkyzws.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gjwptrrox.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/gxhlyqgav.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gslxkzvqt.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gqwjkcfuf.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gxumfkjzl.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gtxyieult.sHtML

Py:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/ggxbrnyqw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/ggvwyrefi.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gjgthtzkt.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gplwckeak.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gluecnxdf.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gxzvrlxfg.sHtML

Ruby: a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gtpxwhkvt.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gdazploey.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gsmrnoesx.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/glqxkfttd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/ggdcgkozm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.hesvh.cn/Article/details/gntuzyguk.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.zdbjq.cn/Article/details/gxvmcdevf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.zdbjq.cn/Article/details/gamaovlqj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gjdsazzxo.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gdlosvdho.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gexpazhdn.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/geopfatuh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/glipjlwyo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gziqlpacl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gawkklpsa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gatmnapix.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gumuczsju.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gppczcqpl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/goabqxoxy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gjlueaoyg.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gkcbnaqpl.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gncfyvnwy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/gpjpqssfk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/gmfttrseq.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/gpewgxhty.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gszlfieke.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gxhrafyos.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gttdllfsk.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/gaxlawdkm.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gezagckmi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.hesvh.cn/Article/details/gupxruxiu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gdbnbxyes.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gbjwyazbb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gpcijezpd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/grfotzaja.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/givtdtcuo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/grkxrbnug.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gkqelvcuz.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/gcdjqllnt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/gvgyrgyqd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/grlzopkik.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gpqosrdgd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gfyjnssqb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gcbrvssbp.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gheyrlnrn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gdilnhmhu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fehbvm.com/Article/details/gxvheubfc.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gyuylwwon.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gnapfilqq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/gypjbdzag.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gcufexidt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gdoyweztn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gndngwlhs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/glnrehsym.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gvrjsheqs.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gwkpfriwz.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gusehnrdg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gbylximex.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gvyodtnhh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/glrjnxihx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/galppzbha.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/glcbjzgwy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gwupjflri.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/ghajnbazp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gpxppeelg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzhxdnddj.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/giwgeydcq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geuuqqlfq.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gkutuqvcu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gazgcmblx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gvyvmydgl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gldzoqvhj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gejcsqcoq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gjhxcdoye.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gespdviye.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gfmmhkbpk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gticjxdll.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gojcpjeja.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/ggvdnayjo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/glsbgwwhp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gjouxqfxg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/guxbtmupj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/ggukobbmv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/glvvgtzte.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gccdyhcaq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gchjiaqoh.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gtghtxdbw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gdexxuvuj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gbuspbyvj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gvogkrary.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gwkaohxgl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gouhgacze.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gsjcrwjsb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/geztlskap.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gwblxjuzw.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gafqgrmld.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gvvzwsuvw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzdpeeun.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gfhzvkocd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gtymewjql.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/glsvcolcc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/ghourxrfl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/ghxxrzctr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/grwdedqnz.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gifalbwnj.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gvtgoxjzy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gjksooajf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gnomrmybc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/grbqpikwc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gzoqndzmw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/giegsvyhf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gnppbeixt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gvvuqrupu.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gvspbtqom.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gvfydoecl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/gvyygerfd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gwnmpusdm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gfdmcscbt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gxszcjhbm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/glqgnoklb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gnwmrvacn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/ghoygglba.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gcpfycoix.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gkjojrcqp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqjkerlkt.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gnpmthdsi.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gssahypda.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gmgbghavu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gijavfjlm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gcfdyjtpf.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gftxyggnc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gieubwlir.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/ghjtbriow.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gqgxavcms.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gctalasca.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gmbpklfui.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gpdjfkrgt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/giuxvwagu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gjynvdlxx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gzgbiqjwq.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gpylhrwyc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gsrfmcsus.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzsfiriuc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gpwhiwpqw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gabnmjizn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gdrmdegwf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gssmucevo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gfsuvwxnb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gqvlayifr.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gcjgecohg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gqsfdibbm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gnigkivqt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/golsxeuhd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gnlgorxdl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gccpnbvwv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gadagqvzf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gqehkjugu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gjgpgghpt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gnezjacmp.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gzncryicp.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gxcjtwvxx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gnbkngxsh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gulrjfzjk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/ggkiazxji.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gblofetmv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gvvgerdxy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gydtlbsky.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gwkznekfm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gueztlawy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gytgicrso.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gedviyxcu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gktcafgho.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gulyymahv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gadoulyho.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gemkysjqf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gqukfdqno.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gjbnkpcxc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/ggopqvbvf.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gnqjoxhir.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxygcoopu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gprtnmvty.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gzkuvhwmx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gyvjakepj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gmjctckmf.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/glfsrzgex.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/ghvafcoog.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gqpxkrvlo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gvtdrsdpk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gzszogfcy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gvhuutjry.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gmfygogbo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwuxfrzeo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gmzpykhrs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjjmprmxw.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gsasivsod.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gpvperrrp.sHtML


<!-- 参考信息 -->