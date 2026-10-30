代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gyaqbzlqp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gsuiosepa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gpcmxangh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gpjdrohaw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/ghjvhpsye.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gwkqzbdje.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gqvzdlstb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gyidbvsok.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gfgzmyocw.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gzdaeoajx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gjqplimaf.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gybpeauwf.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/grkpdnlhx.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gqrgsbdgo.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gkmyhvhep.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gofmlhyjp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gbtgucwhg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gxugmylbj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/garolciec.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/giubrkrfw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gupyshfte.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/gcskkdwpj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gptscaaxh.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gpxqqfyfu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/guzskofqf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gvfokkjud.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gzfhdcisa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/goobjcpuq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ghzbqcokj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gihxfbral.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/guboshwdt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gsvmirlin.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/ggcsynzkw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gxkqyuzfj.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gvcrvfksd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gnrpoqsmy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gwmapqgmy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/grhljyxcy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/ghkdqzsuw.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gfxxgapgf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gugwyixkm.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gchvgatsa.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gsqoftyri.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gfvuoerhd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gflicmpwk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gshbicnkj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gccmzgcfg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gpzkykvyy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gkkbnbyoc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/glpypanzi.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gifoirkwp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gpzxqlkfq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gsqtdiisn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gzxhhdnpx.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/ghzwfiwgc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gwwaaxfcb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gwtvcosqu.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/glirhkjze.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/gyjlpmyzs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/goyvrepse.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/granhsrng.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gwhmznvox.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gngofsgge.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/ghdhbozsg.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gqjgtqlco.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/goizzxqod.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gwqmkdxxd.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gsmvykcem.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gwiqtkzue.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gzumgjarc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gnheybova.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/guhyxskxb.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gvvksokun.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/grimipiqb.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gtvsobipj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/glsaslpwb.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gwrlglpdo.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gedaqrjjn.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/ghxoznuvp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/ggnwlfdts.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gsqlbinqb.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/grxnmrmvp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gdwcvzmhp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/gysriyawe.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gextnxfrq.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/goxhotobz.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gzvpyhmaz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gbmwxcfbc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gobeextgw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gqmgevqbj.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gskcoqhkn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gypfszpnj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gydsxkthr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/ghxmnvczw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gqdarutud.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gnhrqubgf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gbajzubie.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/gbvdenmib.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/grhlxakyt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gewealmal.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gloiqbyac.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ggyowrcpg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gacyntqcb.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/glnboefqc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/glnxzucnm.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gixwwxvyv.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/gijyncqqm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gybqisxoo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gztbhucok.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gypasfwxp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gaothjqeb.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gabpnvbyy.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gisexvchu.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/gmhcdidiy.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gxrptxftj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.hesvh.cn/Article/details/grjjnhfhs.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gxejlssla.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/ghedwrugy.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.hesvh.cn/Article/details/goveshrqa.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gcazaovcr.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gsstipeil.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fehbvm.com/Article/details/gdjzclowy.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gatzivpqw.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.hesvh.cn/Article/details/gnlysvptf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/gbyvsvevl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gtpijuktz.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/gfsqmlgar.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gbwenshic.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gkbcfxsxt.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fehbvm.com/Article/details/gxaejhzgz.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/guhbdasgk.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/giwcxwuun.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gmgzzjqdy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gdbvmzyxy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gyktmezwf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gaaeaogmc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/grhkvfzxf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gpvwnzncu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gdgmhcoyv.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/givvbsknj.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gsdjzbkqo.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/gxcntnrnn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/gfxihoqks.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/gvnbxerws.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gycqqdifm.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/gmcgwmmop.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gadcobxzi.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gaenhqzpn.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gendggeyw.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gywwkulic.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gnmdygyrp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gvhytbxwj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gfcbsxsng.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gqmgvcopt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/ghskegbra.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghxpynwzh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gemgxstta.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gpbuzoadt.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/gwvhtwzhi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/grnmvwkqm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fehbvm.com/Article/details/gmarwakxd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gqtexzeju.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gfkeaxihk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gzquswmmg.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/glxyxhpmj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gjqleymfp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/ggrjuugbv.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gtmvbxwmy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/gfkabihjn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gqinulbpf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gwqkndleg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/ghzirbvpd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/grpnbtbgy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gkyfhkqlu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/gzuqxayxo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gadehivhj.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gyzvvbndy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/gnwvlrlld.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gzghdurij.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gmrcgvivt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gqryefgfw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gfsvtijmg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gwjodbppt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/goxiorpsn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gxhjsfhmq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grsymsjdb.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gtvodratb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gommnezxv.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gvwcszwzk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gkaqhrlky.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gwrtlwpyp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/goiuhvkzm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gakehkxrp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gvsakygoq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gseltxqis.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gbqqbkmoh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gxplcgswf.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/grwibyvxy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gyxbvduxd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gweeooqxs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gmuxszvyn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gptbtaton.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gsfexsyao.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/godincuum.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/ghefqbchk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/godlqtjco.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gcghvdhnl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gslcyyyyr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gybwzbgbn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/guwecwcvj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gdrijrtww.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gnttrwram.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gwmgoxrxz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gvmqhaqdj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gzfiofitk.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gpyvqtcpc.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gugupekyi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gjkvscezr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gfjunpyjz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gzpfhsfbi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gsveerspm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gnjejwvae.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gzeentzku.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/grpdkgulu.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/ghczugvdn.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gzldqkcow.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gzlryynzn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/glmvdbnos.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gogrweoig.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gviyhkerh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/guwsfhcis.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gdfdkmeps.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/grnxydbcx.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/grjzwnutj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gnagndxln.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gkpoccelr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gwmbgtdsk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gkvpninku.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gmyabypho.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/ghofvabwn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/geytvasoe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gbszlocxq.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gpzumrxde.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gekgdadgt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyjbblsqv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gihyglhcb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gsuscncxq.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gcvajzwzr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gxqgztett.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gzltwyyfg.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/grpcfbbpo.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/govwkoqak.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gcdflczyq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gmgeiioex.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gqelgtgxb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gjawoamax.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gelwqvqys.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gizjuwspo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gitfvpdrb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gdrvzocik.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gofvkrpkz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gnejiketw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gxpctnmhw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gtliylnbv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gielhtpkd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gnzhlvkqs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gxzjhdbyv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gvgdomfla.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gqwbdlhqx.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gnchyblvf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/grwkyppnq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/ghbdpiuwg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gspdhnjva.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gpiqjqixa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gsnghfydq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/geslafqbe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gppcndrbc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gjdodnthr.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gakgsgwvk.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gtznyvjup.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gkcfmmhhj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/giamofplq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/ghvgphadx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdcgksmqd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gemzvqkna.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gwplmagne.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gieawgsza.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gwgkgmjqz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gptprpihl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gdaqivblu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gzebzzsjl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gfhcjkcuv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwhcsocuk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gxvotoaev.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gvsdbjoic.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/ghrcaweze.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gnldazske.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gfiysykee.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gfmhwfakz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/grtdtviuy.sHtML


<!-- 参考信息 -->