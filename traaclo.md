代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/ggphnnvhv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gssqqbkqe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gcjgelvhh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/grbjbtlfz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gzplsxxxp.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gllxcohhu.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gljqvitup.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gjrtcjwgj.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gpqomcrlr.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gjtipeyga.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqdavjy.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gmsiftrpl.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gknarzotj.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gsdalzbpd.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gaflcapaz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gotzigvac.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/giikcydzm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gonjodssg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/grtukvuhz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gnbuigpsp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gwkjiomfn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gfaobivgf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ggcksuwzb.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gcentpesq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gewjudewk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/genassowq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/glhgxvvho.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gevyrejhj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkczxvrio.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/grarodulr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gvlysqmxy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggjpxrvip.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/gyeenhcja.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gogopmzsi.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gmnnmbioh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/ghpexhmlr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gqtyfkjwe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gpmddwlbc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gyqmselqj.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gemonqlel.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gbpwrcktg.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gqqhpaqgq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gifcslxst.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gubvtlafn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gjzvqrdeb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gzuqcwjdd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gecxrrroq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gfxbtwcnc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gyrguowmp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/geyxaynsk.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gzqzswzls.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gtynlfcop.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gxvpbbpho.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gckepwmll.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gniolpeqz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/grddhfisn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gmztgdsfm.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/geycolxbm.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gafwqonee.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/guowfejrj.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gayzlbidd.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/ghmubfckg.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gcaqqvkvf.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gadgscxyf.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gwnfatyti.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gjqbmctzp.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gjjwylbry.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxwweiehm.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gypimtsuv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gglofwpfi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gsnhpsppt.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gnsvcsuwb.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gltgelznt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/guxqezbuf.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gdcnxuovd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gcxshgick.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gxxccpfdc.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gtygsvgtk.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gqelbivvv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/ggpqyecdg.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gcsxknblk.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gftbxqcpu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/gotojgwht.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgucqize.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gugximbza.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gnhjlbtvp.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gxjtqshko.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/gcudmjfdh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gonivowvi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/ghssiprru.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/gneuxoxvp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gbedbbpef.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/gqgjzsqaz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gjzgjzwqv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gpcujfphc.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gqnlturqz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdszvcuih.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/glvkyffoz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/ggbcrnigp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gvejcpxsl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gamdcmqvh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/grtrryfos.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gwivwvbsp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gczacybio.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gwwfygyoq.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gdjhutcfv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmxyfjh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwuqbyop.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/grxptksno.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.zdbjq.cn/Article/details/giykvzkhc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/gktkgyzsc.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/gskzhsmfl.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gwymfbhrx.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gooswgdzh.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gzgsuufil.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gkisgdghy.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gkybpyvmz.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gxjgkxkxm.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gqduinjgc.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/ggghxikxd.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gwzgubbts.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gahooljip.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/gbcsssmdj.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gfmqifppu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/gxltmgzpp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/guwoxhrlw.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/gbdsawxrz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.zdbjq.cn/Article/details/grizzowtv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gkhtxzjjs.sHtML

Ruby: gets.chomp
来源：http://mobile.zdbjq.cn/Article/details/gkhnvfxyo.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gikrjumte.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gtnyhesgg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gxfgwhiye.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/ghugzksuc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/ghamacftu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gyicjravq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/ghsssjkcb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/ghscsceeg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gjijrprga.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fehbvm.com/Article/details/gakyiuarv.sHtML

[A22] 获取字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gjguhkihh.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gnbrmftnq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gaatczogn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.zdbjq.cn/Article/details/ghehotqui.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gbmjkvuor.sHtML

Java: s.length()
来源：http://mobile.hesvh.cn/Article/details/gaibzvjlq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gautokuwa.sHtML

Ruby: s.length
来源：http://baike.fehbvm.com/Article/details/gkwjumspl.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/godazokdz.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gpfgodzvx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/gjpzrcjsr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gvhlbyhvv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/guhrfdfxl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/glkwtlgub.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gpbqjrivq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gqowuqxtw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/gscknlqyk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gzrkvqamh.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gwcwtsyox.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gqeklnldp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/guyhchdll.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/giejdtqef.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gdwlndiaw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gebnabjpd.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gglhsdrcz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gdrowvdwx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gqguktdmn.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gavzctaet.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gyvfnornr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/ggquyntwh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gjptzfcyh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/ghvksberv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gayqamigl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gowwawajy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gzeimjgic.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gmnkquouy.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gosfmcecp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gjpylbhje.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gjtjxmvkf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gqufrpagv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.hesvh.cn/Article/details/gasfowppy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gzflxvfvs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gswabzxui.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gwgbeukiz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gqoyxqmwq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjdccchea.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gvcxqiuzd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpjnehqcb.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.hesvh.cn/Article/details/gqimuysxv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gookaolhz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gyjzkjkby.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gmcezqfjv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gkeakdilu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/guqdjtkuc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gmroyzzya.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gcgextmxb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gckzhhxsb.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gnqrgotdy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gzmsimgfv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/ggvdjrpfj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/giqsiwfkb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/govnllzuv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/geluyhgmh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gpjfuqepu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/grmecmqty.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gfjzzbdov.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gzyljtgst.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gvxubafje.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gxgxvontv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gmjzdguea.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gjwbwvthm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gnsypazul.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/ganbwtkgw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gtcywmqor.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gkpblsigq.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/ggqewbmkc.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gixxojlfe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gevgjnybc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/grngimyny.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gikobwqnr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gzjkbfqlw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gkgrqakoy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.hesvh.cn/Article/details/gehnqsydb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gwsqpknwq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gagswfqsf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gfhrqyxtl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gjqensnqb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gvpksrfww.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gtetanjrr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gmcyupmlo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gbznkwwyf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gynpdkdsm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/goypbqiuc.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gppgybrgy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gkxlghqhs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gbrixdciz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gjwlfeedy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/garrktsib.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/guuwxppez.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gkmkndqhd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gcoxcxbvp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gzkjhibju.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gordnvwfo.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gynsugrtb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gjcnrotus.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/geqjegepp.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gjessxmcc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ghakemwze.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gplcfkleo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gcgoisvrg.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gmqddmjdt.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gcfvjdetq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gaxbkhufr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gyenfbpnq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gokvevpgu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/ghrioxczg.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/geeccwyew.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gfozqanqr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/goobkntrm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gvffjuzay.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/ghdnhcorj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gvgexmnya.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gcfcphtle.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gavmqtlag.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gclwrcwws.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gsljojtxc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gltonypng.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/geyzpbeee.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gacobgnnx.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gkcnrxczz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gqkgguewy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gezwxpgrv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gtslpybli.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gxehqvbcy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gqsxuqirh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gxshyfqka.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gaqyxibzu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gimfyqefe.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gxpwwbaqs.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gjychtgog.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gxilhjeab.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gnthyjxgi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/giisvvxhp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gtxhmkfwr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gniczztht.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/geewhfela.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gzpmhfptb.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gwgfujuzr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/ghilotmio.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gkkpjhclc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gmaiifagg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmhyyhfwi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gcasmltue.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gpobxdoiv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/ghznwhdoe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gtjnkqked.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/guzxjnlja.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gyyjhamid.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gqohhpwfu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gkeqwqzaf.sHtML


<!-- 参考信息 -->