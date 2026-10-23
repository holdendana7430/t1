代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3zsmkxnxi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pexqkodc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wfxsxbst.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ravxjjvm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3udlmmtpi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rxcimjky.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3orwcuslm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ktztnnqy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hqbiywsz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ydcvqqap.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3emmqhtcg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mtgcbaaj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vixmemut.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hkxzewab.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbpfsho.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3tlxxbolu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3edvyeksh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wesgidpn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3fspyrfeh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3udwzrqtd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3dtqmekii.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xycynxdh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nbybwuyu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3spdkuebg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3prhwlzyx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jflynikb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3evaegaxq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ljiyydwx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3woihuzfw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kcvxirae.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3wzluhjqe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eguvfohi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ecmneotb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3llluxlnb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3obiwquga.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jxombcyd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cvawjemp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gligtydp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvrecml.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sblipqbl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bcqevcxq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3adadfatq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3gfqzfhtj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igaqafak.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3wfmewejv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3nddqyphy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3rdqdweav.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3imuzsmjj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcavamgn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lxlundjs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ltrhapyk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcmyqkl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3viksibha.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3tfkizpia.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3adqnmfte.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rojpavdl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cuwhsqai.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tznexmte.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3htvuluqw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hvrwktvg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wdpdvajs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ybzwlxjl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ilxhazmj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3gmmjdvoe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3timttrap.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3geqmvljw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wbxknzkd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3odbxkreo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oypevqxc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lyuzhcib.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lhayxwnx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3nnrxapkz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kqwpvvgm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wogxgvbx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fcqgxlqf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3okelrims.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fffeliem.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3stfhggjn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3srkanthn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3buytobzj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hftidapg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cgeeezcf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rddfhjao.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wtovojrh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3prwynyhs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3lutdwifi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dkapcyrm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kkutlrwo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3anncykfz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mjbdzzrx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3apteczvn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bvaazuep.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cnsiyeol.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uqsklpyb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xqziexch.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqipmcym.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nwhtkhrt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yuedlnis.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3mblzsljh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bihncplf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3mzzbwxtq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xevtjpui.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3addbkymy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgwbkjzc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3eoqpvvtq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3cfbknmzb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pgkjqxjp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3totudugc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3evkupknz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fuivqiwh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ncmgugeq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmscxajh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cwatxdiw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bbkwbslo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gpiyikvf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bprxwxig.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3dcpviwxj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3snozcayr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3noqqqkye.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wbnljpnl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3aakctnkl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ngpdykex.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ryvcbkgn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kirrxhks.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3bfzyxedk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3nnucwzvk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jkhtylao.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ojmabibi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ssagcafe.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3orgqttue.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3sdsnxbgx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uripqult.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uzdiuvcs.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zkhsylkw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hislnjzy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rasvjdem.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rjvaicgd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3sjuroqew.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pouswtxv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3hanmkeiq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3hqgombze.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wawuyatz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3slpiihrf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fbhtkixs.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnxquktv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qugsambk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpreqzq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzylbtr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dvupokto.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fquxaxgd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgqsovl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cuqcagfj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wsnfpzcv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kiestqzb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lynucpkc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kggskhrr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3avfcxmlg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mitqhmth.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3lydxocgo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iqcvlnvs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ttnuhwuv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3psbfdzht.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gghwbjlk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykovyady.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ijggvhpz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3itfkhfou.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nbbskyhs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqnhamr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mdgpizbt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3jiqyiqjl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ixqyfwkk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nerbufwp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mcjxkeum.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mddolhxw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kcqgsqdw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ntehujwn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nijharpe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ouaxvans.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mmlscrex.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dvnmmgtj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jbhoktyx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrgcahxd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qyyawvai.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wshfdnlk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3sonbfdlu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3otlfnldr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ysmvfatw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tbgrpqpa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3whtesonn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3quemlitv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3vcahjicc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yowuxdem.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gjnjsill.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hjykasbb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bfcatwpv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3saypuorm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jxuhcjsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xicryggw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3aklnzgij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtwutejc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3foavoxsw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3kafknglz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vrbymbrs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xodtucvj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3adugyjjc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mwydachs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uojrroix.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3enwkzqwm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3svjtfupy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vnggeusf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xongxcdh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqmxrdxm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pbgejuaj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qdmldmwt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rvxydxgi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zsotdnih.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qfqglzfc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hzhwtpyn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3maeeywzt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jtxdnhgl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3unpnwfdm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfacpzkv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3madpclso.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvgsudux.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3edmlutoc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tdibovoh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ilfvbpcj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ijspunbg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vbrvacfo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtbltdhu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhockhs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fknaplde.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqwbipwe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fzeypfhh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3udcqrzyp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppkgibjq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mkfkcadd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yllecvef.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3opxinnss.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xnxbpidn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qktpvxju.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rckatqto.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3awortwmg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pzjveabh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzbxocpl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zuzwsidp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wsnftabh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uazmqrkk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3opvtrhnc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3esnoptjy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ljcrdjvm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wqefxfpl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mcgbwuqj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvoecpyd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3naagbfeo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3utzbtcow.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cntpuzzp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3odasxbqo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3quudapzx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fglnjiid.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xbfbeovz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hossskjd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mygieyaf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mswnrvbb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3iwebgbud.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ypyrtett.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jxicicdo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fyfwkvek.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aqijeahn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3eweegyqx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ltjikpxj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3biryklwk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ifxivznc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3sxzgxlnp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfjsafxq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtkdjgma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvtvggdn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlfuulyr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qnajyndx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3scusxrlm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hvgmzvxy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hdfjbmyf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqfqwwy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfntavpo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ooofjbxx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ncubewii.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdpjlugj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3glzxmxyn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tkxoginj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3utknzzzp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bxtrvypq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wicjranp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zaqgudek.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lqwixloa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cloemedq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmxrdjff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bhdjtsmv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hnfsaaox.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mgwjppqo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qcrrhsnx.html


<!-- 参考信息 -->