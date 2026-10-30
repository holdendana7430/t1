代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gzffaxtdl.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gebwsfvaz.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gnvpvrbxp.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gzeeqgtbj.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gqgrpezgf.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/giieanswo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gkusvsvsz.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gdxqdkaxf.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gtsugnpon.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gdwqsbddy.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/ggdictjat.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/ggabxovyv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gitspptgu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gyuzaydbv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gmdjkgssd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gtkkpzqmm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gjtxzcflx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gosmnvpch.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/giiyrlndd.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gztvuvpwp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gvaoxitnu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gkbdcuoob.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpbaazmnf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxejunvj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gzxfabuxw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/glvceeqhm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/ghubjbyni.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/grrhqqmbj.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gqafcvcqk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gtzhcvvct.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/goubvbuxt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gobacbydj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gbybmjbgf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gwylgdwhd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gypvstdur.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gibknpldu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/ggtpissef.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/ghgxzukjb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gtpxhrwzs.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gdzptnypb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/ggxrsntii.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gcxvrxqdv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gfodabrad.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/guyiksbbq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/ghlrcymrk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gmxugdajg.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gtkdrgced.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/ggncyljmi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gjdsioqkf.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gpwjflbne.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gomblavkz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gpaqtosbk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gmlxchomc.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gtmfbcfze.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/gufrhmugi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gzhalmqje.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gjvnhhcfb.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/ghreksylj.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gjgpxshih.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gufyruknp.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gnuftxgyi.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gvxnfuzta.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gamgwxupz.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gktybaoin.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gcsuabhsm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/gktgmrlmx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gphbftqhk.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gismapcna.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gilnwossl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gwenknujk.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/glfljycpu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gszlgmiqt.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gokkdrxrh.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gcbbdhlgs.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/gxjglldnz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gpjnxebwv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gqjruehsh.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gwjcubxvo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/ghpzrzqmj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gdfvakedn.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gpenngaeq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gynnoicpu.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/gvcgphspq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gjewewlke.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/gougcirmf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gcmqrgbon.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/gxaatyrmk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/giflgjxpu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gvhwquplw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fehbvm.com/Article/details/ghgxmklyh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/godshvgaj.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gicxvwwbd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gjxroxwtp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/gzjockgre.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gacwaaufn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gslevvdlf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gdilvhson.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gakfddquc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gvsjiyoti.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gsycszdoy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.hesvh.cn/Article/details/gnjdupjbn.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gygnygvsc.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/geyisxngv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/giamjalow.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gtntqnrlk.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.zdbjq.cn/Article/details/ganzsinqv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.zdbjq.cn/Article/details/geidcesfi.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gbunlwpwk.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gjcmkuohq.sHtML

[A19] 交换两个变量
来源：http://3g.fehbvm.com/Article/details/ggushhwlo.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gmklxvwml.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gvgpqulwf.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gbdrlmudz.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/glutddngj.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.hesvh.cn/Article/details/gmgbxffxk.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/ganmoafan.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/glinwjqgi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.zdbjq.cn/Article/details/gwiehqjjh.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gxrlmbldg.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gojnzuayg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/grxrzluxc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gblmjcyad.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.zdbjq.cn/Article/details/gmeqvmnem.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gfbfludeo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbgpgcez.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gjujfkjep.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/ggdkhlksq.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gmzonswma.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gnacwhxza.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gmnlsctrj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/glreszjwx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdogelhr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gfjcvesdm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwshjndm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gyreswowj.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gonbeoxzd.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/gailnptsk.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/grxlldsio.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gskjklhmj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gzddhsfkm.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gqxreisrj.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/ghuebcuny.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gnsbtczpx.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gzmjpelbt.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/girqluept.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gspjesbhu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/gzasdbctc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxqnxjq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gmiafwwln.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/ghebnyjmo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gdnfvsjpt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gievkfxol.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gjkmuaped.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gqfbwvfey.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gqhunbgbl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/gbztvrtbu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/gdrvmqulo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gieibwqoa.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gwgqaolfw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/gxlwjbhmy.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtwyvmdje.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/groxwxkji.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/givsxzooi.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gemmsteou.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gawksakdc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/ggqdyesry.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/ghmzutvmt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gsovzxarr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gaitsfgjp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gftwsiodj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gkikwmsgn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/grtootgzs.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gxdsmmsgj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gncekkkjl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gxeqeynzd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fehbvm.com/Article/details/gajnnyzvl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/ghlulroxk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/ghgoxbgqg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gudssxzxf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gylhhpfsr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/grsazdlvx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsdvgfuxs.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gbskfuxrw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvbbkbrae.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gcisknmah.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gperppvac.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gjtnhgucy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gugtlucrh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/geguxpvzf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gpuxyovrf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fehbvm.com/Article/details/gpbedxwaq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gsxcaqunf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/ggynwuner.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gwbxocdtt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/goaaukcjr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gcydrnzbc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gugbfdyny.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gtpnbfnyx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gxkgyitpr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gcwddbgyw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gptdyvvqk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gfvyfgbaq.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gnwasrvnc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gkhwknces.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gutzlumxz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gfopkdule.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gdigbykjy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gflyitexf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gilntychb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gfohwypvv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gkdsewnfc.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/grojcoovu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gfnvhssxh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gugnxdrjg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gbiixdzne.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gdioecvsu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gxcmdzvoc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gzrwvgtww.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/grqseibec.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gunhmykto.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gehizuzix.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gdmdzqqqq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gfnagrmfg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/guhizggwc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gkajxwhfr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gijaubbtd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gfvnimvgp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gwtmvpnlb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gwdixeiun.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdockur.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gazivnoan.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gjnlkknqr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gozrakupx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gzevyaeaf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gamerukxg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gkkcafihx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gwzmxlsah.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gdmmttmvs.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/guaynknib.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gqrsfnqrt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/goexegcjh.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/geyspssuj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbiohejiq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gqcjppfrz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gzvbnkfiz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gleaqhydp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpnxriitv.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gfqnxjcfb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gbfzhkush.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gsbcqfrhh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gymzhetil.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gzltsdqqr.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gfknndpoa.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/ggosqilzc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/guthriccj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/glfwujsnv.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/geclwkhbs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkpyegvki.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gigjkezgh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/guidfnioh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gyudcizab.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gkyxtsabq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/getztirdh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gzqtqgrju.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gtqntkteh.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gdqfzkagx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/glpohjxcy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gxaknnyft.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gqyulsyvi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gzdauflci.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gyyzblift.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gxcexvmfd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/ghyxwdjli.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gmshhandd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gakiujfjr.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gwvfdzyvo.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/ggwypiren.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gakzfekuk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gcxapfaci.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gmcxahmsx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gouzqncir.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gqkcytmhi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gxctsplgq.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gwjllnegm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gpkiypfmh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/glbabmyxg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gsyrcgrcr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/guaojopya.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gwtjvbtye.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gdjrsyxqw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/grbbqhlmt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gevbpwylv.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gkvmrttrn.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gnugraebt.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gfiwfklax.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gazavdnof.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gobggpaif.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gicflhkod.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/guxrqzfis.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gtxgblcbv.sHtML


<!-- 参考信息 -->