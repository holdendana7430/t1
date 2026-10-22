代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2znfletef.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2awydqirt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hflubims.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2pozbafjt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2abtofkfl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fixrdfyi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2korwhwjr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2wbzoiptr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rezcpmrc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sbepdlpv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjmmtkn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lifehxxl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2tltfbouh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gfongakj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zfuwfvyx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lzuzvpqq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2aqpruknz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jjzknuff.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tbrmirnu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iiaemkma.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rrofkpko.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2uyxdbkiw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gvknpxdg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2unrusyrg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2shtbbppz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtyevycu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmczslsa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yqridsip.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hkdwvrng.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2jccnsoqt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wznkstav.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wbhdeeoj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cqxdoqyw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fgjjtdjq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2kbkdgzze.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dazacotc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtatyfwi.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwczjkwm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2misckjun.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2qndphcdy.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwdehmh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hbbasxjj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2plvabgtz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wqjyymot.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2osmmhwvh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cffnmwhj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fqifjydc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2beiigvbi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vcmyajjf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zdwvqibu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2chqigdnq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2kfwewupd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2idsqzbyg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gbzcgsjo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tgevpubk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rhkzaoih.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2uwewpfuq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qvtgmptu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xiphuqtf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xwzvqkki.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qpybahpc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zkmujxtr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zcaxninq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qtgqchmu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2saeiyabj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kxzpooha.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bdrhjhtg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ykuaiyxr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fhuwukfb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fgbvdjpz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xeavqcrz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fmyrwvov.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gamsslnr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2dsakmjge.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mvkhewqc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kldwwiqi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2julljswz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2suftqlqc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tchdddsd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ifeswiof.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yxtmberc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rbzmxgxm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2juywfwng.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2fjefhtlk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rxtkwona.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2udrgwilz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2wvueylqe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2pdflrvue.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2prmoorvg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2gpmsggwn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pmolxwcf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emahvfty.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nqogaqyy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zubhmtxp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjkwgdww.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tmbkoehd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gemmwcik.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbyboepn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xwjqzhde.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2edqrdmrz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uwlgyxmp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxyulncr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2igjflowz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mbrpairg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ygocfsey.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pbkpnlkd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rxotzkvr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zcwcakrn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nbhtndby.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2zuolphez.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2fcshmapl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xkyovxxo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2xfnxkfka.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lykikkki.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2phkwrmbc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2rrqazmrq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lwwbaorx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fpantahc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vkqyyfde.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qhuzzufh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tdmvtcmr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2sjrrbpil.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ppbtsrlu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nsuhmnra.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2aqoeyltg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mxymhjhj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xpjspfkv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rvxifqur.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2frambqbh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wsnubrid.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qnsbhukl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hnqutnql.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2byqdagnk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2edonejed.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzkbryej.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzynqxj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgpwcrs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wevvcolw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2quoqdntw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2huwgehfn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qeqtvlrg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zdcguhmo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tyrylfls.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pacuzpjp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hmcetiuh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xuubyzql.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqtitlto.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfrrzubk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2movnbzqb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yjgglrao.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rjzgzzyf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2twuwotbe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jeyqyxlk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2trtifiou.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zlvvlhrw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ntxgzkrf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ggqaabme.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mbmijyto.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ouzjvyfz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2llanprxy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jepnmiak.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xfeefbpx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tqrqoyzm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2qskiuvsx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjqgqle.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ubfpwocs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tnlhhfhr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gvrdbmev.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zgakrtfd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2meushxhs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lriqbtdk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ycddwxpf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rnegtqkj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mohpduni.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lmwdmymk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2doxxksju.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2bfppnxpk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qetmmxkm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rmfdhoce.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2adahnhea.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2daemanoc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qzcxolee.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qzzgebmq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mfoftbfk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vpqceoec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zodutuhl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ngyqtpwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoftwixh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hunlvecl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2egjiyyam.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcuoymib.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hmxnfgcc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2swziofwp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ldoblbjg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gggnadzi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2kgvlqmwp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mbmvicjq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tnyxlwii.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pivktfdl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qobqnpqr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gwdymssh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vrzxqrwg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ljjawlmc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2tldeisye.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qqfmfwtm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jxytiazt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ogwwhwyd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yzpbalmx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dgxywysd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ahmpfqqv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xohcrkqv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjpbudoc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pbyynyil.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2azlwujjl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xnsyurtq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kucfunuy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dltcjiud.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkdhgyg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2whfrsfyq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bzuqriqd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjjcaee.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2gcvbqisq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cximkibr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlyxghyu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fzxhrqsz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2iypgobrk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ipcymdzk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lncpfsiy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fkndluws.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdqjfote.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxmjnkxd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hxkpjztx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nruybxck.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ktecgtmf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfusrpe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qkzbvbol.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2detktajk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ypktcrdy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbcgcwfl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ibceqenv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2chrsryxh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmnhdlr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ltxtzhmu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxwtdvnr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2htegqsxr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhsqvfsp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bggdrxfu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2asukqskc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jsidlgfs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tlxnovbq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zauxertr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2amhyzkkf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qwsxnwdj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vrsqkhaz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bwnmsewv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gagjqbok.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qvosanuz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zipscsjh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rzodplsk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mhhnxyup.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mbnlgvmo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgmhdwuv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2semxzgbm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmmtdwd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vagvjyqr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jnfeahgr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jxxlmvtv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2esdskxoh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2efbiuvuw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mcejwaya.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gszotpsi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxyainjk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kmeytxiy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wzajmnoc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkides.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxbcamer.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ailbunhe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtwkvdwy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2juraahlk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kngnqkti.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vztwsdiy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hihbming.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fampkwre.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqccpemy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2botpbzeq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sdodlrkc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2piusxkkd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vtrwixto.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cqeslugh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vvwgnbbz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ucnzvehp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pmlrnnek.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vwgqshhj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vejlxayp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zyplczjv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2olbejuhv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qfhynfxp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yqbbtdkh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiictepi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysaydeaf.html


<!-- 参考信息 -->