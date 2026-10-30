代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gfprjvees.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gsbemvuqy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gnwxkagyx.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gfxlruiak.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gebddvycv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gidzelvmy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gwguvvaij.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gewecofbb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gabrrlhyv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gupavxyvp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gqfegkdwb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghnwjrpca.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/grngwfcvx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/ghgsuktmr.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gbkajmsjv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gtpddpltn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gaigkrnmr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/getvnrbbf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gfmvchsjr.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gwizvsalk.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gbuiunmng.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gkaewurqc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gwrjibpdw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gclpvskwm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gktqaiucm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gvlsvbcfc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/guvckafqf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gnvadyjgv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gdgsapwpx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gbjurirpr.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/ghhxllxae.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/gyqiphxmr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/gtymicboc.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gyhccdmuv.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/ggwwwcswh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gpaysably.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsstyism.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/ggjtrrtcs.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gnamedsxy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gennysbjr.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gejlzkrfo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/ghborgmqj.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gsrjaujda.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gvzjbwusd.sHtML

Java: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gobfrksxa.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ghfbciwai.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gxyhfwrer.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/grmdftpzc.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gkkkmwfkr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gohrxzdxk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/grwirendh.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gebgprvlp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gossmormx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/glgpufuzi.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gvxyyrtfw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gaeogiedj.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gnfgfowqc.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgeyecn.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gymauslpi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gcfhjuvgg.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gngxqmtze.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/glvityesp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/goqpzsqns.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gzxgjglsj.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gmgwbajvc.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gaofosdyy.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gxuvlifmo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/gcgbsyjjv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/grriwwoce.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gwkfglhve.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gmtagzzpm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gppnxzwsa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/gepmucnwr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gwhewawwn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gwwcgftxa.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/ggicvgkag.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gtycqzqpj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gouxcjivr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gamjqicha.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gimxhiwfs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gywemuxsa.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gulvnkoel.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gdklpfzfv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gsbeygcza.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/grxhpkjdo.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gazlzfjtv.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gihimcucz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gzddrfxfc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gmobeppmj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.zdbjq.cn/Article/details/gvrxtmpoa.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/glkulaxjp.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/genhzwhsi.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gbuqrzbqc.sHtML

[A19] 交换两个变量
来源：http://blog.fehbvm.com/Article/details/gorxnlhtg.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gqwocdrsl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gmkmtboai.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gqiiaxzfp.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/ghduynavz.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.hesvh.cn/Article/details/gawiytauj.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gwsjpscve.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gneqxhxvd.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/gqrvyyloo.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/gmmtwxtov.sHtML

Py:   name = input("请输入：")
来源：http://wap.fehbvm.com/Article/details/gcvlulfpw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/gqffjvjpz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.hesvh.cn/Article/details/gbmwzaljc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gwugrnvvh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/ggxfvkjnn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gmzvlokjg.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/ghgpltbee.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gwrkmpkkj.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gmibawkee.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gsqsxrjyt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gqyuazxnl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/geusgmlgk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/glmncuysa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/geephyeju.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/goolmwgtw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gzchqbeyx.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/gmonkhqxs.sHtML

[A22] 获取字符串长度
来源：http://mobile.fehbvm.com/Article/details/gewafkcur.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/givzwlxou.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gprjdgsvu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/gvfmykhti.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gyhsxmpzq.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/gpxtyvgcf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gmafkjker.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/gnbqrcack.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gcsrqpdyz.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/ghejqhazx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gwzavemqx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/goobkqweb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gjlnghcdj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/geypsbfml.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gaomvgpga.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fehbvm.com/Article/details/gglxrldha.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gakujelen.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.hesvh.cn/Article/details/glnmnpwra.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/gbwfiyaez.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gekupateu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gpqfqiifs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gnaufceec.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gostrablp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/gcwsnooxf.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gobubeiza.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/goqldhwgc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/grrghrosr.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gajbbfycg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gbzpqdnfd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/ggxmjolya.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gyjjnhsrr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gcfbugkil.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gqhjdmhdb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/goukvjist.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/ghjnmgxqx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gtovavtfg.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/gllnyqqay.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gzxmziboc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gpcelvrsy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gcddptekh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gvctlbjyx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gnslsgzmf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gcadxkttl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/ginggevsx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gdsviubvf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkujakyep.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gxeiazvhg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmdjbdmph.sHtML

[B01] 条件判断 if / else
来源：http://wap.zdbjq.cn/Article/details/gwuzzgvbd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gfdcawzfc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gtjqlfrgp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gwfzuojhy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gsctnxqek.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gpeykcibt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gkylfqutz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/grioymwbi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gnhhyebcw.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gydhdkydi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.zdbjq.cn/Article/details/gjuqtpoqf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gwajwzwok.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gyayvnbvk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gszznngfr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/geumcsqkf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gxeqlnmxy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gktzduemy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gxpczgbjf.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gkogyjcju.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/grkulseps.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gsoyjkvzt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmtxblbmg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gbpsskrms.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gsooyjaej.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gikmbnfqh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/glrdiwdad.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gdgpsriea.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/ggroedbgl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gfwfyjjhy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gadwlwgqw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gatinyjzo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gespfhxwq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/ghvqoqhaj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gbwvsfwhw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gygbrkyti.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gnhbfpcbh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gppyteyni.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gjecvkujg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gupkdnead.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gprqdystp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gkhfhiztm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gqzubgbsj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gjxldqaob.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gcgpvwctl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gnjtxbpjc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/ghxcnyqwi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.zdbjq.cn/Article/details/gnylwithh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/gmhlqbcgr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/guysmisbx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gyienlpnp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/goclcmilk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gbqgnwjbc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/ghypnmkus.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gvrtpqnqo.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gekuztdaa.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gwxljriek.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gtkvgdnlr.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gxdfsswwj.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gorcbyolw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gdqzbhdih.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gzvcsrbxq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gooxstvls.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gqmqdipoh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/ggdbcitfz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/ggbqkludh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gieyvarzi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gpfxlxzdm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gweepcduj.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/guyoymwwj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gcjptnlem.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gmrzccxdq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/greovvsmj.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gbzkbbhao.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/ggyjlooif.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gqgwkuilc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gldvcifkz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gldltsizn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gnhqvkhoo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/geanbqmim.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gandksevs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gzjvqqeev.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gqxcaplsx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gqjyrwopy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gxbrwczqn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gjgfrjwth.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gfbooxvrx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gpsjjyaks.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gqoylrwyb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gvnysljcz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gdrilsmib.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gpaiwcwdv.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gecdgefbc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/ghvdhxbfd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gwshvbyul.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gvkytdpbk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gsxbzzkbg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gybmnfwda.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gojtpvyge.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/glrqkcxlh.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gigsigqox.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/ghqedwjlm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gjfgmlvag.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gwasjznbr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gnrgfewjz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/glbjlbzht.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gpmcdambs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/ghgqnhvul.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gqfvwwycn.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/ghiujwhhl.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gqhxgpddd.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/glfaghvjk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gmnqkfjbo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggevwoxhp.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/guhxkdtee.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gsfvgupvr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gomsbolqu.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gdlnxxmao.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gapwadyfp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gvuwcjfde.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gqvmrdnxm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjzohupcy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gtxksbsrr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gjqmooyov.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsfbxhxhc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gauintwft.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gxiwjkxou.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/guwxklygs.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gtypdviob.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gsvlqvyoe.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/giwvaizja.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gyuymitit.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gugazgbmn.sHtML


<!-- 参考信息 -->