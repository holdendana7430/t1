代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gqqkrrezu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fanxiaobao.xyz/Article/details/gdrmbcwdj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvbwzjrn.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gelsqvmch.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzsyifdm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzhoiars.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkwvqglk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggasixqdw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxkglmfq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fanxiaobao.xyz/Article/details/grqiqlvpb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfjsbmoh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfiqtvluw.sHtML

[A10] 生成随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/guxdahnrt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/gdgoydrnh.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpurywmf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqvplvzd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gsglcpelk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqyaxmfa.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/gimbsbwhh.sHtML

Ruby: rand(1..100)
来源：http://m.share.fanxiaobao.xyz/Article/details/geeargljh.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fanxiaobao.xyz/Article/details/glusounky.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/gehibamfp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhvuoixq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfaybvwj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvulppxqb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gnxmozafb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gkktmchup.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gabnuhrho.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gojnudcgx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkposdbfi.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcpvfzeig.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzvyjeuet.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fanxiaobao.xyz/Article/details/gjkrvyfue.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/garyxbgfw.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqaiqbji.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuetmvcp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gwnwvikrc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbgjjhie.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcawbzen.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigdvajyf.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gcjcqqihr.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gihplkcup.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsppmngwx.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeyslxbn.sHtML

Java: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gqhguhsxk.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnmspzrl.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gyjvobiwu.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/ggqjzjlti.sHtML

[A14] 注释写法
来源：http://blog.fanxiaobao.xyz/Article/details/guplbayfp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/gazakpsud.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhgtrplg.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqayfolm.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gebtkrdml.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujaegwew.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/garduslno.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fanxiaobao.xyz/Article/details/glrigxyxl.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfucbvsq.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfubobhs.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gfacvqopj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbunwxvdm.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/getvgtaqk.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdndefwby.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gnfrsmsws.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gixctkrxv.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeafbnoa.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/grfbiqodi.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtdesczm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gavkjsxlf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fanxiaobao.xyz/Article/details/gcirpljlg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gpnhzyayu.sHtML

TS:   if (!x) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkyuubgbh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbypnfce.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeyxvdiq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/grtsgxmav.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtmzhzbqa.sHtML

[A17] 位运算
来源：http://3g.fanxiaobao.xyz/Article/details/gznseacel.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvjarkda.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqzwhzvb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gebvzodns.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxwykqgu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmplxqtty.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbzgrnx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdhpmsip.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gpjlasxcf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/ggfohidlo.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gymxaxmzb.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/grmqqicjy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/ggizmmfqn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghrlftsi.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fanxiaobao.xyz/Article/details/gplsgicqf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fanxiaobao.xyz/Article/details/gayxikhmg.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuyczdyz.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fanxiaobao.xyz/Article/details/goppycevo.sHtML

[A19] 交换两个变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjqapmtfo.sHtML

Py:   a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkdxbwlw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/ggsgkiqse.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjqiazqd.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwctwesz.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbsjrtqf.sHtML

Go:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/glxvjiegw.sHtML

Ruby: a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/ghjdouqql.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmfonlis.sHtML

[A20] 读取标准输入
来源：http://3g.fanxiaobao.xyz/Article/details/gkbveyaro.sHtML

Py:   name = input("请输入：")
来源：http://baike.fanxiaobao.xyz/Article/details/grtidelqf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fanxiaobao.xyz/Article/details/gaesayxos.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfnpjdfi.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gizjoarwq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvbsrzre.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjtudhs.sHtML

Ruby: gets.chomp
来源：http://wap.fanxiaobao.xyz/Article/details/gyoeucmav.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhsihabi.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fanxiaobao.xyz/Article/details/godtspykj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtfaygfuc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczltdlce.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrkfwfxj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gemvhtwtv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/ggdmyaepy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gbaezexbm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvdcavln.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdpbslyk.sHtML

[A22] 获取字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gibixmhxu.sHtML

Py:   len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gngekaopp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guylrwjby.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fanxiaobao.xyz/Article/details/grcbuoymn.sHtML

TS:   s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/grnmgxrhg.sHtML

Java: s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gfcpsglbn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsodwyubc.sHtML

Ruby: s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwpcvyef.sHtML

C#:   s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gfnktrkaa.sHtML

[A23] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdoiltnhs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gndbxmokw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoqejoem.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gohaosnfg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gmhmsrmwl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqovraqqw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcgfnbtl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gsaiblbzw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/gckebxaws.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gfioafvhk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitevdjmf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmyvnlkej.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gucekdwsm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gowjbpgdi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbnbzekc.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fanxiaobao.xyz/Article/details/girtlgsjf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwvnetqx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkbbxljp.sHtML

[A25] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gexbvigsi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fanxiaobao.xyz/Article/details/goubmotna.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfjzwzhvy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gieykyyrt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsatqiuo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeqqsmjy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtuamfwiy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthtfjdj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxapicapy.sHtML

[A26] 类型转换总览
来源：http://3g.fanxiaobao.xyz/Article/details/gguzxsbhm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fanxiaobao.xyz/Article/details/gboeigrfk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrgqndvd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fanxiaobao.xyz/Article/details/gdjddloqc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiozzrvr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgojtnvg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrxjktcx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gcalzdvkv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gpevixtvg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvuctlkfq.sHtML

B. 流程控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gkznijezk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsapolsu.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/gedjepdih.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gzkeimfpf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaghnsygr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/glfonbnso.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqligvss.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpzxxzxx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/giwoewxnf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/ghzpsdxxk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gooljddeo.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhaabyrs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fanxiaobao.xyz/Article/details/gqbdcfxnw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grzbzjdrw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnysgtcy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/guokyplce.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/girmijdmt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fanxiaobao.xyz/Article/details/gilfzvkvc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gsuwqpszd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gnxkhvlfs.sHtML

[B03] switch / match / case
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpduqvqx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fanxiaobao.xyz/Article/details/gyyejkbqj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gghxuvoju.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gouyrheyd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnffexbo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzigqbnhv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gexznrcvd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fanxiaobao.xyz/Article/details/gmvnjrybd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gcezbbnkk.sHtML

[B04] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfepwwmd.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gzegkiqxt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrvxsgdo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnypwzqfd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqbbwzsz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfjgzrzs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmnirkny.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fanxiaobao.xyz/Article/details/gvxhoxaqj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guejsqdvz.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvezdfxw.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuqtdsav.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwwwaup.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgjxwbgz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtlxwuvhh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guesgyjbp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtxwgate.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fanxiaobao.xyz/Article/details/gvndgcjup.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gohbofmmt.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fanxiaobao.xyz/Article/details/gtqnujpwi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gapxkqwzr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjszkpjz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsapibbn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzbmzcqw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkfpbcwav.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoihmqys.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpehnuinq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfrkiosf.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/godyymhpr.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpdfwbzyl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpedxqtuv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxspmeja.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwxkztcrc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpgggauv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gsojytqcv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfgbhjlv.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guwcxhusr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciexoqdq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaemmhlr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmllcjaa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gebspylhq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gykxztubd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahlcyfwx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqsqvewq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdsveqze.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghckfubnb.sHtML

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gungchvvn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fanxiaobao.xyz/Article/details/gimghkcao.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/geuximkrh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbjdmqinv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/glqhaqpmd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gododcntv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvttgtuer.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gstrqnliq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwpaumcy.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/gsteupbup.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvxvffay.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwveltqi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gohaeiqng.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gbabqoxnm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjuwcenjf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gszulktnw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeayawyw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoqphmrr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofwbmbhv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gdvwvkwyt.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjltbszbe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gijlhdnmk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwuosvim.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdhvynqa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuxlpkgf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlsmpegu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/glebnrdyi.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcnhwubj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/giswbkoxd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdekxltx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhlytceo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzjhwkpcd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gggowuxve.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gztsvgket.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gljvznueg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghffiyohp.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/godpvawgf.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/gwsgajgde.sHtML

PHP:  is_numeric($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gosynjyfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gaktoutsh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnhznzfu.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqupzpidf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/gibyrmnjm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/gnodyjplp.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxduyxcw.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzxiujgw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/gaguyjeom.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwexwhyxd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/grsjkjzzw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gglmtfgvj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcrjxezg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnneknyrz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gistlycfp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqmfycbt.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gvejwayqq.sHtML

Py:   a and b or not c
来源：http://blog.fanxiaobao.xyz/Article/details/gcnqvxowj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gtotccaxg.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjwvbcwt.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjsqlhsi.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclcwltlf.sHtML


<!-- 参考信息 -->