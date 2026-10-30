代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gqlhphvrk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gfckgjxyk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqabtiqf.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpklepou.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gopdklxaf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoiomvds.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gijczagok.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gptrmpqzr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gootecplx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/gifcduncx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfbeynmn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gopbnmbot.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gweazmqaq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/giorqtraj.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fanxiaobao.xyz/Article/details/govqcgciw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gfbnyxprc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklbndtyk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/goknivuxx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/gvbwzzwle.sHtML

Ruby: rand(1..100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwuutvmt.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fanxiaobao.xyz/Article/details/gjubixcmx.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnkmoqdh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzrzrlgz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gzgbdrvbv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxrmzyfo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnkygalw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gfkwcabct.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fanxiaobao.xyz/Article/details/gnsayqder.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvxcfgzm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/guoanqygb.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gccguuyfv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzceigvpz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdncjautr.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gaslbmvij.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjmmyktg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmfzuebx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlszuwwm.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/grjohhskc.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagzlefn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpogvgpb.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gczezgwhe.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdxldzyc.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/geypozqwb.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/glhzyoktd.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyhaftax.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gndpqwbaq.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzheipary.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnudilofx.sHtML

[A14] 注释写法
来源：http://baike.fanxiaobao.xyz/Article/details/gvuuvunfa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fanxiaobao.xyz/Article/details/gurhjmcpi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbgohgjs.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gxxbxisjy.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxirnkwfj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviwabzdm.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhywourk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcixdgpn.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gicxyenei.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glivmoobw.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddwegyhm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/goiqlqaok.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghifnllrq.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gcqbjfrwc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fanxiaobao.xyz/Article/details/gsemorhox.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiburmpt.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnvlectg.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gvxejmotz.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gykighfbp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gofalqqrc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fanxiaobao.xyz/Article/details/gwzqjklxb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnqfezkp.sHtML

TS:   if (!x) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gynvdxvbh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhsvzdig.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqjrdopu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gimgmwaho.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/geshppcmz.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/glzkyvqgb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gszabwfws.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgttybxk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnipyjxv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmjmkonm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcrbubyy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gqibmncil.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblogipqq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnnuifyu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fanxiaobao.xyz/Article/details/gvcjqhmxf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmctdgdij.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gyvbgeauu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefzzcvqj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/geatgdbua.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fanxiaobao.xyz/Article/details/gzfltsrqf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fanxiaobao.xyz/Article/details/gcayjzpmc.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjewoqhv.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fanxiaobao.xyz/Article/details/ggasrhkoa.sHtML

[A19] 交换两个变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxsoqzzph.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gmijnrzdl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fanxiaobao.xyz/Article/details/gwwjopgmr.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gyuluisqq.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fanxiaobao.xyz/Article/details/guslenujs.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqlbuonw.sHtML

Go:   a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprhlnaud.sHtML

Ruby: a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gebrmzlup.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fanxiaobao.xyz/Article/details/goqlqystt.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmifjcltk.sHtML

Py:   name = input("请输入：")
来源：http://3g.fanxiaobao.xyz/Article/details/gtyizqbeg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliwkzumg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdkvhyjo.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfkdhibl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/gjavkogtz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gippzbntm.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiivozhc.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fanxiaobao.xyz/Article/details/gegjwigdm.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjllmwue.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnjpeoltn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gljckbyxv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjjfwpgo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxeyqobii.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gskoynxor.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/glxinjmcl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdhvexso.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugwkmyq.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcupglikn.sHtML

Py:   len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjhjkohj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fanxiaobao.xyz/Article/details/gvefqemdf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fanxiaobao.xyz/Article/details/gxsnqvcxg.sHtML

TS:   s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguykgbrd.sHtML

Java: s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/ggpumfrnt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ggitbaugk.sHtML

Ruby: s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gpqbwoenc.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypndgxfc.sHtML

[A23] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxojhzjxi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpajdatp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gitroaajq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/guqzwlakb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gfolbyxio.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsvmdhpm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fanxiaobao.xyz/Article/details/godcjqhxo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gkfewlyjb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/gazgvlyzg.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gfbhgkahm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjmnstnj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gamvmafvu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gououmtne.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwyjafmh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfszeeip.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gutzwkbkn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdctwvsbf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtachgpvi.sHtML

[A25] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghnmdcfqh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhbofezr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glahrbirc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gufcerdcx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxlygrci.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/genmytosl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuqpfqri.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoqvnlvg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwwvrzpw.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gcbrvqayi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfzdmjz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gckztltha.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrwxscfx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbhstvpt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluktcgqk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnmjjvjp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gqgawtqhg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfimafrrp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrqmtwwb.sHtML

B. 流程控制
来源：http://3g.fanxiaobao.xyz/Article/details/gsfogekmy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghkvnwswe.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/gaieqbbne.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggltdoqeo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkguvogjh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gughhmikx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcofwctzq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gabtnpyat.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbzoopitu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fanxiaobao.xyz/Article/details/gdtnxiili.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gcbjiqpum.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fanxiaobao.xyz/Article/details/gumwdvqxb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fanxiaobao.xyz/Article/details/guebfgtfd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwtufwin.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmktfoea.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/geffyzbtw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhjxwaxb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcateqhuq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fanxiaobao.xyz/Article/details/ghyetzbdi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/glvelejcv.sHtML

[B03] switch / match / case
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbbudexk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbaztyiu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbpuxjvzz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gewspbjdw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gajqrsqaj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glrswmlnn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gakxymmgm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fanxiaobao.xyz/Article/details/gqxrmbuxf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqpdzoto.sHtML

[B04] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gdkhwtlhy.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gidizunws.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwosbbvn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnanfvfxo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gughqadfi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/goutoencc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/geoazujsn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxpyuwxf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkqcvkjt.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gplttmdij.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbanujyy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylgenhur.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghridzyli.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glqppolss.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpucqdaq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbqjbnvtj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwukefroy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gingsuuco.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fanxiaobao.xyz/Article/details/giqnmqfqr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpgcdxpp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdturbqqf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gifkrbotm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gawytequh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiyphlge.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gajwnbgwv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbiunwp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqlnvxdr.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gchewyncl.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsyqyvtx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsguifmdg.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtczwbsro.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjqbghgi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkakcphfr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqttqkc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdzanarm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbxfffvl.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvfjfumj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/guulpwmod.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/guiiytdet.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydmwcjme.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqdapxfv.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/ggljwqthq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gueirywpx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfgczcoq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkzxyjzy.sHtML

[B09] break 与 continue
来源：http://m.share.fanxiaobao.xyz/Article/details/glruwnnfg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxwxhnbrw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnpkuqrb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqkgdsus.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiwtwdlx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwexdqtx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gvcjdkwwc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/gahliadfx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsyxpxmz.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gafzzvfjz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggartizur.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfereskzm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gfufqgrnv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/glxffpbmt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldnhwfht.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsklxgdz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gtehbrpif.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwgmfswfk.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnxrqofh.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnscoujy.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehclmnal.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gjgkmnhye.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjxdfqzk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/grmpggvll.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtlgbawn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fanxiaobao.xyz/Article/details/ghrnycnzg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhpujkka.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuemdalh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/getmbgdvu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpcagmyy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/glmnacxwq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoogigdw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyujybcho.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsqrtehu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/grbyvnzdq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmqafxm.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gojxggrep.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjlknzve.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxluyjtkc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/giodfnplv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmemgnps.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvmiydsp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzgdcrfr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczvpyudt.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkbhrgky.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyzhptvh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggharaaie.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grddybmkb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gfobowmuh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvwkxiov.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwazhmbax.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwtbjdcj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/griokuhte.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzmxcqie.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrqulzzn.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/ggfvnjuix.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fanxiaobao.xyz/Article/details/gifpgdmfq.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gufiigbfo.sHtML

TS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gntkhtsty.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzspmawb.sHtML


<!-- 参考信息 -->