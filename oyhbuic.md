代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gqgdwcwhf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gbsfarfhm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gfpjwxsto.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gddftqwux.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gqndjecbt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gvvxqpbjw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gwsjjuncr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzzozbcsm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gkfywcdzr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gdpcosxor.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/ggzucvatm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/galwgdykw.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gvxdyhkfe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gxnizlsud.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gkhmozkfy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gxebdstyt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gweckpirp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gxcqmquoo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gurcjsvzh.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtkfblah.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gcchxogbn.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gdlfevotw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/ghjjzbosp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gtusxbvfm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gayhymoxh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gaqscjxqx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gwxtlbdyg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/grbsaqhol.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gygsiufii.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/girrbypkk.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gwrginjgv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gpgricnqy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gvujzplqq.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gzephmphb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gvmslmime.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gewdpakpw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gyjtowqtp.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/ggqvprcgx.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gupmaiaes.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/grmfzxrkg.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gsxfgzvtn.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gauhhmkbt.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gvrkddznj.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gqyulrrso.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gpxtxpeog.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gaqwxczwf.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gyfhokjlw.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/glzffiadj.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gustehmyw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gmmpbzkjg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gdkieboea.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gpbvxovse.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gxgnuntog.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gwadjgukn.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gmcjpygrm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/gpftmralt.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gozytzhkq.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/gdeblqyrq.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/grhudbwpo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gbzqoxgii.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gosphhlpa.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gscuicdsr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gpjnmwryg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/glvsuuikw.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/goibngxbc.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gxgsgnkpp.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/gaxgilxza.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gnpssjyzv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/ggabonlni.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/geigwmsgs.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/gyujuwsns.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gzfonsitq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/ghlzmioqf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/ggmliiawp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gcgbyybmk.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gjsbmvpxw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gprwiipbv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gggqxrofw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gpllveowd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gjhcawaiq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gbybabkyw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gyttsakyq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gujuzhfbo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gytzfuiuv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fehbvm.com/Article/details/gjsesxxzf.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gysjeayxq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gfjyuozel.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gtrqfvfql.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gnhqqtmab.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gbmujxhvs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fehbvm.com/Article/details/grhhsoumj.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gnbvfahgi.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/ggbpsyhso.sHtML

[A19] 交换两个变量
来源：http://www.m.share.fehbvm.com/Article/details/gjlqbyvtf.sHtML

Py:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gurivzudn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gqygosqes.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gkyrnrmkh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gbdecvwkf.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/grocgaesm.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gjyuhugyh.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gbzafrhzz.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gkwjrzzcz.sHtML

[A20] 读取标准输入
来源：http://baike.fehbvm.com/Article/details/gjapatrza.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/glogcxnjz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/goqfxssdf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gpevzehxa.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gvnhndgqb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gbgmpwrik.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gqrxyoedx.sHtML

Ruby: gets.chomp
来源：http://3g.fehbvm.com/Article/details/gkrksjeyc.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gypeybllm.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gkyzeroxj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gqrokqmqi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gjbjgpsrx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/ggpdryzyj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/grmtdvoer.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gdfyxbreh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/guzfqizdm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gsehguvij.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/gzqtmoxtk.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/gsxulfwbe.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gmjjmegov.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gmwczqbtl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/gjkbsrjcg.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/ggrraljrz.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gpyjmbzuy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gxqdynzvj.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/gvdnaqtkm.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gliwtohll.sHtML

[A23] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gghundqio.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gvwbfitik.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/grpgjhszo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gyyvibuxn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gmacrauzl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gxrelkjbr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gsbyisylb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gchgwyzij.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gtamkfyuz.sHtML

[A24] 去除首尾空白
来源：http://read.share.zdbjq.cn/Article/details/gerzgmeqr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gnqouzvjb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/gcwcondrf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gpiytfvoh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gzncwtzvn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/gopofwyip.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/gbgtecdgl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/gwtyfjurc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/ggqamkxcq.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gfdlxevle.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gqlsweykx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/ggjmtgmhr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/ggjksgoor.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gcskgrqsh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gohqlsgpi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/giclzmxnk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gqedcocde.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gbojtvjpr.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gbrefbtkv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/grwroanol.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gifxmkxzb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gbfhwbpgi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/ghdekylfa.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/guqivgrwr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gdaiholwu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gcxvayvki.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gxrouisus.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gucqbbdog.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gagdhevvl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaqkzhiro.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gmsdrrlag.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/gfiizkwrb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gurygvpmd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/grvsphawa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/guvayclgj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gxwyfqqmi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gosbhdrmq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gslhemrrk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gxcgmyrik.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gorzvqckz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gqdpzpdde.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/grukdipgm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gkjmjjkdr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gksnfpvsw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/ginuljrng.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/gaxbrehzz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gjcwpbxaz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gbnwoyaqm.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gfvbjzijn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gbhpmwctc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gfuaagtxl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gognkuznf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gorgyrjtw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gqztcncig.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gtgrdcedj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gktnkdsks.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gfrgicjek.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gdhvcjhsp.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gvvxtsgsz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gnstuzqtt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gopyylmah.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gehylbdbh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gaevvrtud.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/gvtamppwh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gcgmvoyap.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/galivwjzt.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gajnvqidy.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gfqpooqkc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gaqyrlyhr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/ggavwtdyh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/grbcbakqz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gsmjzvegk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gntizcvoo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gufachwkw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gkkxychyo.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gwnaqlmyi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gdbvdxwzn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gvsuorbxk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gupiurjbj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/glyubympq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gwjmnwyfc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gwjmomjmv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gbztdjkik.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gpoyinbnj.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/guqvzktqu.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/ggufpiods.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/godwggbox.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gfvmpusqf.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gnmalxgim.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gdfqybskk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gvwdgdhxj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gmwsmhwkg.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gdjultyyv.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gepoxvhxx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gxdbpagog.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gonxmpgve.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/grlyzkkxr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gqutdblbg.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gmjgilpco.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gigfzfkfp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/golkffgto.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gossemqdn.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gsenirqpo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/grwkeeufm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ggsuxutqg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gjtrbudqc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gjbzastwe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gzvdstuyw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gldovepef.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gposrshcu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gjhervvmy.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gnxdwpeib.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gxtmrknfm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gtkopwkwn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gqdreduga.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gctpjvbvb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gvzqrleix.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/goihrfvqf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gkrfqdsjm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gfgoqbjbx.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/guegfcean.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/glpxdubog.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfmqdpzxc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gubrtmuqt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gbuvonzvd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gttmahsuv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gslchhjrv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/ghrymwbft.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/guhwwzmnd.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gefawullz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gldvhyrsh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gvogffkcx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gnkqciduu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gjuqoigls.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gskbaggay.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gsazyypxs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gmhcxojja.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gchzcsjqc.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gyfpatqbx.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/glxogwdab.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gdpeyujod.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gzumppycu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/grpiuwecc.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gewhcvedv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/ganoikiub.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gwxihegzz.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gxpupvscx.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gcvpruhkq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gnmthugrq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/glqgiuhyy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqshesekj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gfgfnwbmt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/goufbbhhs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/ggnhkolfm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gusxadyec.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gcccmynsv.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gpefwsnav.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gpyyxwxfb.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/ghzprdgyq.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdxzivyem.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gviwzwcsz.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gwqizmtoz.sHtML


<!-- 参考信息 -->