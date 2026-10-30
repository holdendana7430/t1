代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gdvybwpyc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gzrzptqvj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gvxgskrlx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/guhmxlchy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/garenxgpy.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqleohtsi.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gfswuszuu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfuaiqpy.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyfwnfevv.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gfmvqhvqt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/golbeomva.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gexmeaozh.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gnhlzctpb.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gdwlvinbx.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gpdgzlexc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gwgdtzexi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/gisbpljxf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gchoyclzj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gxbnnugnr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gqonylzkr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gnbvcvlof.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gmqqlljrq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gfscgfzhr.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gidnonyuf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzpixzfzw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gsnuhobbw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gelmprzsv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gjlxtqvpl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gxolbpqqn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gflremwow.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gnxpiqbnl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqqkrabzw.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/gzeidrzqs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gxzgefzrt.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gvoralqqq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gabukzcee.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gajarujli.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/guzirbyop.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gqnskomxk.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gfwnuinlt.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gqhduoevs.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gbryahtsa.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gogxdasii.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gxiiqfjip.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gbgqlfnoc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/geqldbyqr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gvlgsgfys.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gbsdhkwcd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gcxxtgjlt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gtkbxlgsh.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gvggmzsoj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gqicnfzmb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/geebaeftc.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/goybqavik.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gzmelhowt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gqaatomeg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/ginqtpasi.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gywoaydqy.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gfxefrjpj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gcntidoeo.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gntotxoml.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gauwjfcwl.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gidlircqp.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gxxouzpjl.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gcdweglli.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gepyohvku.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/guuqamgvv.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gomkqnehb.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gghxcutvc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gcfyrjlts.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/glgsweooc.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/grdzikdzc.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gonlkfgpi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/glosjsuav.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gssdhuyfx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.hesvh.cn/Article/details/gmrxvmstr.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gorjsoobe.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gjspqnlqv.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/gbnozlrlu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gwsspsjxr.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gwzutjikw.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gshxdlobu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gvurdqrfq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gdytvkmrw.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gskwcuggc.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gouebpryv.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gomedslik.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gfgyjcjvg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/gapdpthxs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/geszmybdo.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gsrnkkdrb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gypnamnis.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gelxqojip.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gvtakfxei.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gegjpados.sHtML

[A17] 位运算
来源：http://www.blog.fehbvm.com/Article/details/geebtuqfs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gjecnpqkk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/ggshwdxbx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/grhbnarox.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/guuzoyvne.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gksrsfwwe.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gzmyvneqy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gvfxycadm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gxkrsfycj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.zdbjq.cn/Article/details/gidsqondq.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gcbmmsufl.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/goeyfpgyx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gudfmbviq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gytvakbxq.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/gruhpjgjj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/gwzsyjvrg.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gpgpzpbuk.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/gammxtelz.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/ghyvhjcbe.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gwljwifwm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/geqmyqdbz.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gdbczjlof.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gtgsdwnhd.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/gjentfhit.sHtML

Go:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gxujhmbqp.sHtML

Ruby: a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/ggjsvjigm.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gpjfcblay.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/guiodakjv.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gcekprqjt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/gvkaswgzc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/geddvopkp.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/gtltittdg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gopjpshum.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gpjcfjeul.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gtaevhpon.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/guuteesym.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gdqlwtldk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gvkwpmptp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gszkrokrx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gerdgjlhz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gonralncl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gegzizlpf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gtnalikqa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gwumuzwwy.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gixmpaqxv.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxkpmhstp.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gozovanfg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gxxofcrlg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/gxsxujxzu.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gnzxvabrg.sHtML

Java: s.length()
来源：http://mobile.hesvh.cn/Article/details/gdyryqmxs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gzdzhhpxe.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gtpjzodns.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gvxclyctk.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwajmslgo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/ggpjtjlni.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gddnqlgfx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gmtjtfdgv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/ghcxzceib.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gtgwcjfqw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/ghcqbhtiw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/gvcticbwe.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/grxevkyyp.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/goieslrhy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/ggfrsxice.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gkdluclhx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/grogaebro.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gcygbuuqi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gddxunfle.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.zdbjq.cn/Article/details/gggmjtslw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/geawfeibu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gmqkcqgce.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gclmabyoo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/giuaocama.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gnjndgunr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/godxzqtai.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gsjlbridl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gybatiuio.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gydhrkxzn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gqgujwwal.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/ghsdywhni.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/gthnqetta.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gchfkvrbn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gpgiimeeo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/groxlzxtc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.zdbjq.cn/Article/details/gnagvsard.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gqggovldn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.zdbjq.cn/Article/details/gglywwlpc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gdcpzocbi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gtphhiyhr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gohjjufwc.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gjhoaqnfg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbowaryjw.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gourwctdk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gdzoieoik.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/giwtbpqbj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gbarvffnj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gddqzubua.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gfnpvyutb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gieftkfyo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gefovqrhb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gxuxhomsv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/gisofryhs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gjtzcnuev.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gstpmyfar.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gylsbhzmt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gkgllfrgg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/ghvlxocnd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gkdtbwnyf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/gvaoffimj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/ghfqagbzi.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gvfjnvjdj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/gxwlfyobk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gbvzctduu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gspxrbrgg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gzrrwfjow.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gkhyzmcvu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/glugvcyno.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gpcqadhno.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gkeraqgdt.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gzjafciko.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gcuvetjqx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gsfejzkwd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gkadggmis.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkrkbzgl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gofflpycg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqcjmfhn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gesrxatms.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gmkgysaqd.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gzehnqkgf.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gkdieqgur.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gomfmpync.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gkwuzraia.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gwrqzynyb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gmlfqvfye.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gqboesfct.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gpigejbyz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gnnhzggsk.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gglqiamgt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gfhxlqebg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gfaqigakv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gumnzbmwz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gtvqadqaw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gpvgpqfjh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/grsivfuye.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gtlflmtvu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gegsmvwtf.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/ghfjyruwi.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/ghisffqzf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/garkhdywk.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gqzvnmngn.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gbwcdwfsp.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gquuszosr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gfoabluxc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gebacpvyu.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gsmzhhfzq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gythtfzbb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gdmhybhey.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfcbcrxxh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfdpxuqxg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gmctruwak.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gledegzfc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gtmecwugj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gmgqangpd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/grrhmylug.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gaauzspuz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gmqyavckr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gyxsbbkrh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gvbyihkbu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gswxvqppi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdjuoucan.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gbriuslqc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gtubedzoa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gbfjhelvm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gxemhgxux.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/ghbbtzjpz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkjzduuzn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gzsjokmxa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/goghqvcbf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/ghrsuadre.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/ghifgkfyu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gqglftdqr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gwgeadthb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gvbgnrydw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gcvmfxuqc.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gkuetmspd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gbiudecoz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gnkqjmjgv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gbtrwnjxs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gtfsdsecr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gpcoqupkp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gaypnmwky.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gfdouowyn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gbpeviouj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gpawwjcqg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gkeiyhzym.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwteowcwa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/glbjysgef.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gbifvwsso.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gxhdbvjph.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gogzzymxk.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gorrvnaht.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gdjvdmnux.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gfdwydmqe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gcpiloxzk.sHtML


<!-- 参考信息 -->