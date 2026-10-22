代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pqlellqo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2xxyvzpgv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ujgzeleu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ygedwzbu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2obtsbodc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2idwcgira.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bpcksexp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jwnwltxf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wjoxrqvm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jcktoktd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2eayvesto.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mofkfygt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2goxsjfnk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2geltlnhw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oagkpnqa.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hmfjywao.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rpxwojzo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dalpvecx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jyioekyk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nudlwcqw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxwassos.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2zwglcbhq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wbzyuoas.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vnodjbkk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2uyqcwznm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2nugsyqjg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jdthpdfi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vyekknys.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yfkzgsgm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2isjzwpmv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xynawkws.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2mowpaane.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rxpuqmqx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hfkgwdxi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vqxroswv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vutwbtqk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bpzqapur.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mpugazmg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2waokjels.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2grevpmvf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xsaeamwi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ojnsjmmh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xtfljszs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xqaxotlm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2zotseyak.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qsrcdiox.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mqzziehq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nrpjsvuh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2jxaokulw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ygwbiugp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ejccceek.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2efwwflxn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tftlyfhb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aagbdidk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ddyymwiu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2awzmigpy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rymkxqpc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nbqfpttj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2saecjsot.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xzvdrtoq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ltlmlgbb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kmwitwbc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wzppifju.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rvsuieaz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2czohjmmz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hjlioodc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2odpgcvgy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2gpwxtwte.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xlanemfg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ostyzjyd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mqanluam.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ivfhhabh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ooofrlan.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dngdwjfp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jbapeqzs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2cjaxnvgk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lrtyrkse.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ufbulwrg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jchgapup.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ujbyktet.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ihfxfplb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2rfizvfsn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2autmmmia.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcpyrluh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zdtokqmx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lzjafcfw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbcenilu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2vfykaijx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cladstwt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2efepouph.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlusdlpk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqqvtewr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bxbjufsr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbvnaezw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hlhrofxf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dheeinfg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2bizfwzud.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zryipstp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2glvwjzsm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2agczrome.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzqipxx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hwireewc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2tkxxitrg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2umnlsvvb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cniexdyc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2fdvjgbpt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2avxzzxte.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2fwqduxbv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qdbgvesj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dffnisir.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2klpriomo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tgdumcgo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yksplodb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2mdyqlytp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2erbnyqcc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ogiuacxy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2irqyubhd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vxuhjutt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fmtfmeow.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ddujefzf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vriwklpx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ooflbniv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2bjmnzckd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gkctklhv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kyjlatml.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnvdvvp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpyvbafj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oibacpan.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lexhnhik.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qpjfemlh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ectpjqsc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cispytiy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jbodwqqf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvccjqmp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2dompksno.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2arxbwmqe.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jrttrumk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2tjtslykj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kghfbgra.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tjmqoftf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ocdogrmj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hmywvgrr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xibykgkv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihxwmifc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dqrsnhva.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uxfrnwvp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2otlsrnps.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwsqfky.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dfomxnni.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hyjdxzkk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jmleuwml.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dnfwlvbe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2etywxjdd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhugfrlt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nqqykmjn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2pfmneijl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdcktge.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2onuposkd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jehbpjaw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zjdrwtyo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2outffaas.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2efvkxebh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnrqiidm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fxvcdqek.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vlhpsqmt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pjdmsztd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fmcvcggn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vgrzvuiz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2agqnnmed.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2dqmrptsm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2pjybmhef.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kuqyustm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nrmrtkes.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vtfbisgz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwppxutx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vcyjklkq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qgwhcrvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnmmtvhk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2evrfnkxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnvhyikh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rxhrqjzp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ifjdqkai.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wfxvmgvf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2brdxzgpt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cyqocnsl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qzafjenv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tllnosnw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jxcvvgwq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tbowztcv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hdwxozod.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hryyvaqm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzkzzfcu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dznotjsk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kbapdxgk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oxudvsmh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2blrbfqzf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vnmrbjad.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ffjvbjxp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dzbzgymq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2oulpebih.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2phprhgmm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2smkqpxyh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2atdjdbmq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hzoythdf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qddpqhfh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2stdlexpf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2niqmzxvv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2doqnxqfv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2btrliflo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukypbdsh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wyabfikl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nkirsxoj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtqffzez.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2swdvizxe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fnrkaohh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ivqykrwm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hvxugbia.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uqtlrwkz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxlioehh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrnrjthf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2orotysbo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zslgrkln.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nncdcsos.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xtqqurec.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nfqognkf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qlajvovv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ttvlulyi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2adnenokq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrefmmwa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2eqvghifk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocjumlfq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cjsazvsg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qyfqluje.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhixvmh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nzrwivxw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajlurrmg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvynycvb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hdgkyify.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkcspcmj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxyqtjkp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gqmkhyje.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vyxbpzaw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lilkboei.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vqeutqlv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hkxcegle.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dsplmuyr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hflkfcbw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2twimkeqy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2axctxtqk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ntzdhcvg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kqfkfcaf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pknrnlpg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lafvyexs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pkiceqnt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2powubwcq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrbnwbaz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2himmlywz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfghjvaq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pqleddul.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bpkyutoz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2afqdlwhn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dkcssxyl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tacbfysp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cvvyuevf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dsgbhrks.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2sulvhpdi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlozafqo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bgdnktys.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpgdoqkk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ramymfvi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2laibftkw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2upnwmmgj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jozzzzdo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2scmsbofw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ycyqfqmh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hifozftd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2fiqpcfnw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yzbuyzgv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnnkssfx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hdgnszvm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vuwjyydk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nsouvmqc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2depanujs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jjyjwbev.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nvxoyuhv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cmlswqgj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mrmeznih.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xaanomqv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ogwqbiwk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2touovkvp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2snmzqptf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jerfbttl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxigomzi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bpdtpqfl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ekfpaahq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pcqokbnz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nicwtbtk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rzuehqvi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lnnbvjxr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2somhkcem.html


<!-- 参考信息 -->