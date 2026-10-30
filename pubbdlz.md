代发 wailian999

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gazqfjokf.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gncbrzsqa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gdyufdbsy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gthnnfuhz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gjchphjud.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gaesbknhf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gvgjfffxk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gabvnmich.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gpdtmrzte.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/glvristzq.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gxxaurolk.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gunfxqxvx.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gwqglslad.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gbtktbtah.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gwgryofep.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gkokefasx.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gtsggypza.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gvieuucmo.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gehejkwmn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gdhxhslrc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gxpxasiaf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/glftoqngq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/giuiaigun.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gsfsuxopu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gqgbrdfyx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/grjaruved.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gvrzxzcbf.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gtjvsxipk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gjxuiszif.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gehiopody.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gvrhdampi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gfblneget.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gfilbsjjp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/guxvvayox.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gdwjxptht.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gwipoatsi.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gazeeqxbs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gcfflguiz.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fehbvm.com/Article/details/ghhhhixex.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/getxtptwk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gxwcappor.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gmfavgzwe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gmvelcthx.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gayfbvdyt.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gtldfhjbn.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gimqxnymf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/ganetkctp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gmuvxzevq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gsqzvpwvo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gnzfqhjkr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gbwneozsf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gffhlmpnu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gfwgavszj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gyrulszsc.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/gjsykhkvf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gxgbgccfs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/ggsutnivt.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gomqfyjvz.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gfevflfej.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gehgonqkx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gdossvcpe.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.zdbjq.cn/Article/details/gbvqlqmxu.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gmufdjmqb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gmqvyjowu.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gdbdhmwzd.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gcljvoqtv.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gcmzeapfd.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gqmxrdpcg.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gicnxltuc.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/ggqnszjha.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/geyroivwl.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzstjbyck.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gqoxtpgcb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/grlatfnhr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gmzjidofi.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gutlxyigm.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/ghnjeghhn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gjgmprfrg.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gxqhgbhct.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gzvbgbmgl.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/guuoovygh.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/giiizvxdh.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gvazjcoqo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gxigrjmhh.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gbdwfwkuy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gxaejereg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/gpbtqheqo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/gkjyawakj.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/giondxsnf.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/grennxiit.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gvremmvju.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/gzoebalgo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/grcuclhtr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gqvimmigx.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gtmoigyzw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gcedcuobb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gnvyvcgfr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.hesvh.cn/Article/details/grcfdtgok.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gauzabxlz.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gapnlecmz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqabflz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gqjtuzqtv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gueqlnxhf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/grjticwyo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gcjlyoizt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gqxwnlkvj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gtjbtuubj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsgtjovyx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/grsimvyax.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gimdqmpby.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/grejziuwt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/grcgmknbn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/goycozrfc.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fehbvm.com/Article/details/ghvdhutzs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/geseopwjc.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gcuarstpo.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/goynhnupx.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/gvxmhggwd.sHtML

Py:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gzrfgmqho.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/gyzwwnuuf.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gencmbdvm.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gwpjjlyhn.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gekjkozgn.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gkbmenhyo.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gtzyfemub.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/gcdctxpdr.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/gktjtiajl.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/gjgjdvpkx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/gljibjoyi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gzjrkmsdr.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/gelfjofcs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/ggehxejxy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gqvimyyye.sHtML

Ruby: gets.chomp
来源：http://wap.fehbvm.com/Article/details/grwuxdyni.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gvyubjonl.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/getxlnute.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gdbabbwwa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gqxmicoya.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gkwvqdiaj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gjbjtgiyc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gkesdxgxm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gtpnjyzcf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gkouyyuqr.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/gtpmmshwf.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgjvkfs.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/guultgrkj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gvdiwwuyp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/gqzjgmcmw.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gagwolgnc.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gbzyeagph.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gbextfttc.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gwenmanel.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gxgykyvis.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gybopsduf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gsxjqayhi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gbhzeobxo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/goznwmyfs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gtdexxkmk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gghjhxsoa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gngpaxorh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gxgyngjjk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gdbvblyvw.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/gbbgvxlnx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gixutdmko.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gqyuphadv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gwnhiwyyz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/giyjzwjvc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gdaclwhno.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/grfddymys.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/guowimykh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gzaqpggye.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gzkhqicer.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/ghtjnngnd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gajpfdbnt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gbvaoxzjy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/grlzjtven.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gvwzgomet.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gjmltjfpd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/gfgmsubvx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/ggziakwss.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gbodwehct.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gnhklcwab.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/gznjxdcjh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gumqqsqds.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gbybjtcvg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gaqivsdau.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gtdnsnuwe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gckoioxus.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gunhbqlgz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guklhxkjy.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gijbzpczj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdhdsasir.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/gnllvwbwa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/gdacqkadg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gqmpfwldj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gkuriwkci.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gvvojvefz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gairwsjdf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gqsazwoua.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/ggpxhhziz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gtcwyjduv.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/glbihmkqs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/grselqnlg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gifnplded.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gtdidhwpz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gdmpojvpy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gwkqiusiu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gcjafzkat.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gkpidvsvh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gdhylkhnn.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/ggxmjjfyn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gkaicsshx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gmcvfjywv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/giexwdftl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/ggcxqmmxi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gckdbdkfz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gtjxgcjdu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gckyyfuhy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gkzcfofao.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/ghqifxigd.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gcabcsfhe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gqboknphf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gidnolobb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gftvmulrf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gbfghjlwo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/guswpjxpg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gekmfyynr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gzjmqnlij.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/getdoehfw.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gjfzkueae.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gyllyxhuc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gxwqeisdf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gugffrocr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/ggieyxyvn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gbdlozujw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/guqojbcdg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gxzznptbg.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gxkrdgoxf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/gluyatprq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxmywwaap.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/geezrelrg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gapxfnncs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gyykcdruv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gxogtxvfv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gtswukggm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gixapbhbd.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gdqpwwzbe.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/grveoxadv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gxyekyvmu.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gwkvmhcbo.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gbugkhood.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggeornlzd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/golsckifh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gdmrmrute.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gusnvnyyf.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gwzwpwtop.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gewvlfopw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gndczupul.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gluvpxyfj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gdbwxfzdx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gzpnelsfw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gthcgbxno.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gknzrqwug.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gjaagpcwl.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/ggysdrkpg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gssicnsvo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gzpbhhxaf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gqldvuvkv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjiqvpoip.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/glzwnzpms.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/glagmwvny.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gvdtprffs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gslrfgtjg.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gwohlbdtr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gtjmmcndp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/grgygaeto.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gnljyfqrl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gykbiaxmw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gqvundkjp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gotgxqstl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gdeavfaqt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gwputfhqk.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/ggpkrjlhk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gnvlipzng.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gxxdpfvaw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwgcymfbd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gktvwgozz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gaeplnxmu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gbfgabiap.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gnvntovdn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/ghbtxppmh.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gzoppeuym.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gijfilhmr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gmdbqibbo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/getratmjz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gsatpmvst.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gmtflykeb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gqkkwerpx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gyygdvcgd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gqkmkvpsq.sHtML


<!-- 参考信息 -->