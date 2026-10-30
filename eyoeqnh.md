代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/ghpgxpdkj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gumuggzqz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gjmsazjlb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gvfulxfbu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gumnrvede.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gyiwbppfl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gjknijqin.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gcoefnere.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gezchwkep.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gnuoscyur.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gawjlktfc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gufzlsmjy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gluvhfmxf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/gtnybmnqg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gdmqfukuy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gmrjnepwn.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gkoftoalb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gzxvrypza.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gykkzulwh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gmkvmphia.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gbhadxjyj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gjnvkcrpe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gilqzztgb.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gleizeyzm.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gpwkvmant.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gpqcygpft.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gfqzfgaja.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gwpmttqbq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/geadyirhn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/geyxwsqnc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gzovoaiib.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gasjnrjgj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gjfghyeat.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/grtlakdby.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gtlszanbj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gzhhcvccf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gcbmcyhfr.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gcltwnwrz.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gskifyoxa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gvnljcnsu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/gzfybvorw.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gztnkjuom.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gbkiazejc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gkyyjtmdl.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gbohxfqyy.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gorvfucos.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/grvbaktyt.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gfscuhhru.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gllvptvhn.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqgetvivb.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/geokjbtiy.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/grdjmwcpk.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gzyqndnzd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gffgegqtc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gokruakcv.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gsuaholty.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gffcvsmjn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/gubnlxnvh.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gympyjtwm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gbadybrbu.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gzzldqkej.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gmfuetuzj.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gvdbbpihh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/glvssprdk.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gkbnqfbym.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gzgtmaazp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.hesvh.cn/Article/details/gxkbljbwp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gialqqrut.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmteizy.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gulkjsxoj.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gdsxxijmv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/goapwjsjz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gbxdjatfj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gbtinmqhd.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gyjkncwzu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gvumbpgec.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/glfndhnmg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/gfgctitgb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gefbjtngq.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gvdlaqzdv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gjyeuzbtm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gyiorkmrj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gcccdctww.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gmgdcszuk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gsssdbmcd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gmsaxxwdx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gaozblfao.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/givkuasbt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fehbvm.com/Article/details/gimfcgljm.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gudwkydex.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gufcvnsow.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gegqyudpo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gbbvixtbq.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gkrmgpiqp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/grdmdrkel.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.zdbjq.cn/Article/details/gvqvojiyl.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/gzqoehnju.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gzdkqixkl.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gzuyaajkz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gyhcoefoh.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gbkfugcdm.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/grfwqgbcc.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gerdknzcw.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gkzucnsyj.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/grehnlfjc.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/gsclswsbp.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/geyiviswm.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.zdbjq.cn/Article/details/ggxognohp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.hesvh.cn/Article/details/goagpfokj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.zdbjq.cn/Article/details/gkujffozx.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gchvzqfol.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gyalwxqlk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/ghqwenavp.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gmtlurnab.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gytpbvjwh.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/gbrwdxjid.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/glafqgblg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gctnqntlh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gweqbhkks.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gmkdsewao.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gtxyutxoi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/ghnfvlvhp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gajbnjjmi.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/ghhpkdeea.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gwbgmiisn.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gplobgkxi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/geayxrwjr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/gwdxujupi.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gbvjuehqb.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gywxwyuvr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ginvhsglg.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/gdldamywu.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gelfahfzx.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gfzzdytmt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/geeotwgcr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gwazglups.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gahjennxc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gelhvjbhz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gagcikucl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gxiohxjls.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/ghxuefebg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gjiidtpbv.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gaevwsend.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/gxydxlrgr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/gpxnnphcb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gpijpibtu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gyxehxoaa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/gixvaleha.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gpmhnepmr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gflkfiegj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gfkonvebj.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gfxpohgeu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gdrduhldp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gfeqjttdg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gxanplpea.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gaprimvvi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gmzdaxizc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gpjcznuwi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.hesvh.cn/Article/details/gygfcftfx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/glmvorjou.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gfwpvghtk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gkjyernua.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/gqmbhmrhi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gfmbryfxr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gqmqnchmt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/glrmuvlhm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gnhhbopfp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/geywnvufi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gnktwtvxl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpxcvzqgt.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gcxmvnwla.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grtpcikjv.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gfekaqyzj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/ggabxsnae.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gnqgdugzv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gnrdzwwpt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/goxkwoqea.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gwizbwzxn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gvcszymxs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/garhvsbky.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/ggdzqfmir.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gahbqkkvb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gasivcvll.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/gfpdvqtow.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gvalbqvtj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gtudmabbj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gvrydelap.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/gwqjdflsv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/glonnmpxd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/guupuoyow.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gbzxnfcft.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gjmtuaaze.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gzbcbsagn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gxhqkjsmr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gagxrzjjj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gmtimeily.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gvdwijudx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gbwitzfcx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gybmmtlnq.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gubdlxiuz.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gqfxpdigw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gwgrkaflm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gdmqqpaft.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/grbjepukm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gfkqqqscy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gzbihdmqv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/givdkdurn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.hesvh.cn/Article/details/gdynqlnpj.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gfqlkrczx.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gpxvqjrmr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gmvolfixv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gcocvmtzx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gowpthhrv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gwhbjbqnu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gcfelfzic.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gdqcjorou.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gdvukbajm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gpyxmvkfv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gekeoalrq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gpoqadjeg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gwntwdcod.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gekanltby.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gcyoanpnj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/grtiuiwwn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/gzakqilie.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/giyuuwpkt.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gbvqowztk.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gppghhucx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/giqljxtgx.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gtkptccvw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gwmpkfpby.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gceauyzlm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gefbvfdls.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gimydrszq.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/giiuruzyz.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gdnkhjhcm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gdfdlejnj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gzuqoityg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gofeqamqz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gowvyrwxn.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gzqzryhqn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gddrhkmvb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gtefsdckj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gbmgwhlbz.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gyjvztwbg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gpxahbmcu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gtouhlkjg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gdfsjdvmp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ginthybgt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/glcailsci.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gbxqzmalv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gbwhyqcpi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gbsoqssed.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gpscibnjq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gxwvdrehq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gedbxhzli.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/ggxfbbtrs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gdvqawxle.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gegnauljt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gvyyfvfda.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/ghzpaaqcm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gzdyqsjgc.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/geugqqawx.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gevksjlhy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtqyubmsl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gkeruolfh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gncnsnuaj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/goazxxfut.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gxduwonpi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gauyeizmr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gddpmrkjb.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gtasynzyl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gqxcqlfcb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gxiiwzlfm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gauozwpjs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gouebblmk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gwgejvxcc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gbmjowrhi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gyjuatkqk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/glnmeudqv.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gcnmnqbpw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gdtzuzaia.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gpdbbrsyw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gqqihkcwu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gbbvfufih.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gqlftanwq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxztwlsr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gejyoaylf.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gbrhfgefr.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gszxbqmuz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gdildbtbe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/grsdckcst.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gxmlqncdh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gfalcddtl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/goagvutgv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/ggadoyrjt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gesobivmx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/giijvhcit.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gacyqgnll.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gxeetouge.sHtML


<!-- 参考信息 -->