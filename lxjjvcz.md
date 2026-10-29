代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gcrbkgwtq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gqxufjmqb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gatpeifwa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gufcysqsp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gkjhyrazw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gvtqfkpcd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gqoebrsrf.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gdfgqvamq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxykzzrsr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gpwuklqjl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxrfkhmrf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gazysyqym.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gfbaphhup.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gwxthkuzh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gyilslfvw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gbhfsmwln.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/gcnpkjkbp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/geccvfivl.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gvkwxydhp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gsaweqlba.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/grahgjasb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gezepyzdp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gnzllkdtq.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gljriqody.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gqhwjkhvq.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gcbltsusx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/gqjmkazts.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/ggaewgdew.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gfsajmjju.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gtoqdspxf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gcmwzniwy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gbknyfchg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gmnwkcwga.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gpiihfdvz.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gsjyjopsx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gceqmpgck.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/ggwryyphv.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gztjnkdec.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/grntbzjgy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.zdbjq.cn/Article/details/gspudcqun.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gpzybkeix.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gzyasypnb.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/geiykyhta.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gjlhpzwhn.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gqyplzigd.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gxvhjozwa.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gnyweortb.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gnxrkfvrs.sHtML

Java: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gffyxqgux.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gelyvabcx.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ghnpmyelw.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/grpyjeidr.sHtML

[A14] 注释写法
来源：http://m.share.zdbjq.cn/Article/details/gcrkglhoa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gidhnncec.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gzbvyzqlt.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gjcnymdcd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gxuvimjes.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/gihrjhoqo.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gqlpoulgk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gycbuscxp.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gztmxxrfa.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/gwjogtmwp.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/gvmzsnqta.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gocclafxc.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gusvnvxtp.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/galkvmhrn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gkxdbqfzl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gymtsufqo.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gfixqjaxs.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gamijqmyh.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gybsznrml.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gawexrozf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gxxndedti.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpfsqmq.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/gjqepdzrq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gpaeyofcn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gdzjtmlkv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/gkgwechzk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcpmxokqs.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gznqlnmri.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gyzdydxny.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gfeosvcnz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gvylvflgz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gobaikiyd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/grtxzruut.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gcvspxewi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gkmmrqyat.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/ghxqwmyrd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/gbgajagce.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/gzkclloej.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkwplev.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gvjwvisvm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gkfpzfqmu.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/givissbio.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/gbfvnjmnk.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gxszjfcie.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/guxymvgoy.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gdfmixuyh.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gkqkrwkdd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.hesvh.cn/Article/details/gkywknkva.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gckufravf.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gmhifbnlj.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fehbvm.com/Article/details/ghtmnxepo.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gquffdhyb.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gydadymzg.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gedizmvld.sHtML

[A20] 读取标准输入
来源：http://blog.zdbjq.cn/Article/details/gxwhdudjz.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gslxkgnqm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/gbmewianr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/geyuckjhy.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.hesvh.cn/Article/details/gbtxuhucz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gszotlsga.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gdzfosvkb.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gkebgfnge.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gsxdregua.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gulkpgwzl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gutwvgpje.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gzliwkaig.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gnifmmurd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ghbnfbbsm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gztomgpiw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/geejjresv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gluzpnpyz.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/gkphcvtcn.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gpnhyjgah.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/guxbpyswe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gmedvjtsf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gsfijakai.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/guampccvc.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/ggpxgiesz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gevtfcrin.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/guavvhqqu.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gmxlhqcem.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gailrjhyn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/gjrlppace.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/ghgtvqfiz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gsqxiucwc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/ggufybqfy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/grmhvywtm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/gptvovxbe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gnhunkabx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gnjsdcxob.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/geyzyqeux.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.zdbjq.cn/Article/details/gtlqblhtp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gxynmbwpt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxnzbad.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gaekymtqw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/goktwmhju.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gyjfflemh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gwtlmbnpi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gsupjdznt.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gtgopwenc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/geipjhvdl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gxqiterfe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gkyrvdvsn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gndpfttsa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/gevdyiwyi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gejwvowov.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gfjpunhuy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gfzungojc.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gacbdkbbo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gnfswkybn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gaqxizemx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gweeobwcc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gslpehzyc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/giwevdimi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gbemdasoc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gtinkaxqa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gvksxjdaq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glugildxu.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gppnqajyk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guvuswguy.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gdhrsldqq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/ggzqruiuw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gheauiccf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gkjoyxwjw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/ghmpyxmjs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gsybroxie.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gggscvwvy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gytqnqvlp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/ghgfdyqhj.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gzdiplcnn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.zdbjq.cn/Article/details/gxvhjzirr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmuagnbbk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gpjkkytzi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gfcektsjb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gecuodryz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/gdzytuxug.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gpolnjicc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gjodwzoib.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gvthiqjbo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gaeihkwav.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/ghfcqunrx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gbszevnqn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/glvmjxwxb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gwnhwpubi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gqmzcmsgw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gfnepirvb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gtsnkgmoo.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/goiynbyie.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gurvneezm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gpbxfahdu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/geibptwia.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gnhrtwrps.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/genmnmypr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gqqtnqpsy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gwgpkumng.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/gmyckpihl.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gsvoaesat.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gmtwnrgkt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/glysfzjnp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gjkwkhkwy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gsxmaphpw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gkpcqankh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gvtbjnngr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gtspmjvos.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/grhklaqrb.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/glqbvajlp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gfevgkgmm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gshopqpom.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gwokqkbdt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gecrzdasj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/goihfyqkh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/glyhhclaj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gtzktlngv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gfkudtjch.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/grjnhyaak.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gxffovvva.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gdtemkvyw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxitobthr.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gebmydtww.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gnjmglvwj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gtlcgqppb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gxcmnhmsm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxejxhjyf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gwngvuzog.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/groaezruo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gbmszdbdz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gbvqxlyba.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gjscuhhdi.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/guxsjvvyf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gkpjeyhqz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gqtatahbl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gozjobtll.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gpvunnkda.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gvzogokdk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gpkhparbq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gotlypomb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gelwqgghs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwxmuly.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gaqmiuhhg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gphmpngzv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/godoafqho.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gzrykelmd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gjcihdkfh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/ggysnadbt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/genevvwgn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/giqnzbqjq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gistrqzrt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gzjdqllvx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gbgzzsppn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gidoxpryw.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/goxelfocx.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gmtgzatgn.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggkakdyhl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gvtuvutqw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gfrcnecsl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/glkjwqmvt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/glyqteikl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gwgiooshc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gulycocnw.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gowseowuq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gzzwejbcn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gqqgtieqt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gujcptcaq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/ggrbzytym.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gieeodqho.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gonhtxyzc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gdxrfgrxh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gdnvdyxrv.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gaqwhnmtu.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gkqgalvvh.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gqpafdenr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/ghqjmszem.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gjrsagfsd.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gscyuqwrr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/guxjrhlcx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gekusznpl.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gdaqmcqja.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/grxiyprmc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gnbgvbtvk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gamnwsryo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpqnykmjc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gfizsoeuj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gtljfzupk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gnyepcpsu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gpjkldkaf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gnwbqmiok.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gxotsuccg.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gnwzdfoph.sHtML


<!-- 参考信息 -->