代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ligeajlx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2gqcudyni.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwtapcm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2eoppgrzc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvbugcgr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2twbspmrl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgkgemms.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjtlkzc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udeexwtg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tjachvdz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2xecacdkl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tqbapzgb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2uukyskgc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xuywmyit.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2usxhjkrq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bvopjxrz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2exkfyxfz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvtofyqm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nwxiezae.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2wzhxzyfw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2nechhise.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kqfhogat.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jqlhgxru.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2glmyojrx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lfguoqlj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2epeuhcmd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fvucupaq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zztdzqwl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2srchlasn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rarttrmj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2woeiotsq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kixjuayq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2bydsuhaw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ppseezec.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hrzjvclo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2eyodiisa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lkkonaii.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wxhwjvui.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wisunerq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rwloxqmr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nypvyovy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2whpxkyhe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2znlmjjka.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2axfsupuq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oxjtcfrk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uagpldfn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vgifddkg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mzfupvwu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nflbfmhk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2lhlfxsrp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mscbhlqf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ssvwjuqw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yqdkotln.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2runjbgzn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xplrrrbk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wxltjfdm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2efplkuid.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eoqkpjer.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ehicrakw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2klpbhamh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ydlwrddm.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zjjchvqe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2burukbwl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rrfmpwwz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cqqmtdyr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xoxryneq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nueylecv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kyavyxkh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2xfnmyaev.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jowulwuw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptjualjq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szuuaosi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ksvvqtei.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xdmvumgn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sllafzng.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hdshmddz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oktqynse.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ispfftmv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nigewvwy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gocdloqw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqorrqvu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tjupqczf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hhywejmi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mnrhfcxy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2eqciazur.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vuqzbjqz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nrxqjnif.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2smvsqqyy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mquuxuuq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nrpgxhke.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ctorkksu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2wvjfdtqv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2lasoboue.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2fiirsbbz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lpcispff.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nuykfkxt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iilydfnn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2puljfluf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2jecpnrhc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hobyhyiz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mmfrsoby.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2egzgnoii.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ovomhqpy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nzxtwzdr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2awhoubsq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2agqiifdt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vnkxtrie.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2kadeonnl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2relteftt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jtvahfuo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hdsbwoeg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zyedgvng.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2pjuemhlc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aujhepmz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fbypgvyi.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhqllkur.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nflyysfl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sbxldbjx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hatnhkar.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lyqygxqg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fdyhcagk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzxucesl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2msbfvgcv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tzzojicc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fqaoyxce.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wdfolcfa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2objqcozp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2icbmahcs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bkgrhsjp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zimpwbpo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wlhxpzuf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wpafvmrf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uyomhjeu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rkcuujvn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hakgplmp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zxxvlhxo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2smooahks.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2uhkhfrln.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2enbbmxjq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jgypjwrj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2eysknvyx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bqeuxtnc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2upsnddop.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2omwbhqyt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qvezqtwm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ijfgolju.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sdurnkmj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wxpgokaz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xsryqzpi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lolfuhyz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohnfxlpt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jvpplchm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnchxrrt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rivyuaic.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lmrnftxb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2adwqypft.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tfreggkz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tbdyekqh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hqtspvse.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ielnqgim.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rcvxgmih.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2obyofryy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vhwiyjhy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dgjkliyh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcuaqpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkovurwh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hzwnycbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wypvuhgn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2segvrfin.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rvhafwns.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htvktswi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gpojzdxe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2abepqrka.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gxjzbgkg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tarvkozs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dpvzcxwv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2evrucizd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xhzueonj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kbachvpa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jkthhfqi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fipzbpbj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wuuzshfw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2phdmrhgn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jubxwhak.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vxbwvycn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2japzlbgd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gjjvulor.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dfrtmsqu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uccbbxce.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xatjccnl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cmvtcmze.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wgrvrchh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bdlwurlu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dtgvavzw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ebdfyfrr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hhynezpa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2slwjpkau.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvprzmgc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2flkxhato.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zitqgsxv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ytvppyud.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2yluukeny.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pueyffzm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbvtyqa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jnrptgsl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2bbsaqtsv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ixroatwn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2agxbmyvb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ebxirqzx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwvalex.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jexjtzky.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ggkazyhw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sqffztur.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dehildna.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bcakukza.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2woknwvux.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjjzhqya.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gbncldkr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jtbfloib.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ivvywzho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rtfhlorv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2eohvzqcn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jeggxctn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dougmdkk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uydktneg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iysyecgt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pppceain.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wbxxeohs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yycudnqk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vmvafmcz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmweapov.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vxdeabqn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tiwfiqqi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tgkorjtl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lnqeqcos.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ltlxbpcm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jhkdnswt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2enowngaj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jxocneid.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rouvjfeu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mctalttc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcibfuea.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zcpopjmx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fxnsdktb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksfvpbbt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2awvnlpbc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qhjtanhx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pbfgioqs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rnufxesv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ptdfopca.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxviwuv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ddccltrn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hzggwowk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dglilmco.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmdircim.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mpaaktbj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2opeugqog.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qosegifj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2czhonmft.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zhzownac.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jtcotwlp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2peqwdvqo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wypevije.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kyfsjqox.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ilnglaji.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dzkwzysf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fldrrqhh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lwretsbr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dzgjruei.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2boyqdhlc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mtganpuu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2glfbvbgk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lowpfzrj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dyzxgoap.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hiueebgi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vbcxdirf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ojnjjntm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2eotxonna.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gktidxbe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lvlwarri.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwlnxyjf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ruezjciq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wpdwxveh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ahjkyjze.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xuxipsul.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mewybbgu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2pzwbhyvo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xumfrltk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qvswjwdl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2atxyybvr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sldaykjs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqdecte.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbledyw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cycvjwha.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gelvdxgv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kdpkktpc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gkswphlo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2beuqnzme.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bfsmtels.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2olqornbq.html


<!-- 参考信息 -->