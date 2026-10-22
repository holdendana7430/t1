代发 wailian999

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mdlrvaps.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cdhbbzgm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ekyndqfg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2llzvgwxn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kicwksmu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2caqctjdf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tctbpeog.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2jfpynlst.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ggveypkw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2qvdafnth.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hbdyzhii.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2slghzjfy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2aqejrtbg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2jdjiirlk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2nkqkjwee.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ieppvyup.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2foqbladw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nnnotvdr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jrfcbtnp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sdncoynn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2cyclirye.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2giewdczo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxposdw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vrbgkhpo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dwbefhtr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2zhpfjuti.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ikjclrrv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nkjdjmtm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jypzzumj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2trkxndft.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jdzrhusk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2toofbclb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yapyimte.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rhzilqwi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ntvqofnf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ugmrcwfj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2uqfhkqak.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpmmtfx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2xgizeyfr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqmanyvk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bqeiaony.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kindwpgo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2bbeagmtk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mtnkznvu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nzmyvziq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2bsolzoxu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2hqslagsa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rtzotffu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qzrsbdjn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kvpxnbql.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mjyqlfga.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gfmoknbh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qhjoshjj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xedwuxsr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bijwdubs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2pmiungyp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2uonotikm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cpizkvqq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tkxzypyi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jxczjezv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mggxkgfv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2cxfhnmoh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tbqtunpz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tufxfpdi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2umbazfik.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tjekxaoj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zflhffbm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kszjwohb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hivxrnxs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rnypswak.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2krvbpdgo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wzpdvhfp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kvgnxohn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ptqxrbbc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wglufhay.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2offjpsvi.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kfjfblmx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2cygvhdss.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bqokrcae.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mecppwcu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2shyiikxv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ylarjkjo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fvhqdvdf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gdqpcnpk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2apqumwja.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vrfbacqg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2nfvwndzv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2khtfvztz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2irqiglaq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fqdeyzot.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2pccyrgwj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2epuvimfx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2laftdjvg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nmislwkn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tfrgfhyp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ecbnaxwz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2mvgwfzpi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2oaidjdtz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mgcablud.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2eeirrxgt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jlmvkybj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qhzhvigj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2btinxyvm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qxqgqyct.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dxmfnfvd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2njhbxsyu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mwnisxbx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ryrewhdd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2kskkgfjt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fcigjxoy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqsgpok.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tpifpngh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nzfhsydo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2idmqtagv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yuprqimb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2iwqsbqcs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2erbhxjzs.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2uehqettl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jpjakcau.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rkukedcp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gwnbapvi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ayjqimgt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qcoebhvm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zfojbcvf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gehpzxeu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2zvgjrtpn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2cwnnzyfv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2uodzreem.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pjrpbxqr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ekiowspi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2itoazpul.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vclgincv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nsnvtfmu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zlnebtqs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2beezspsj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ycummaua.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qvrimefr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cihhvagi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfsvyfke.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fexmpggt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2esexfoil.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fvxqqltb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2miaoupkm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2viktyhau.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yesfsnox.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qjabdwmi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2aesadiue.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2vtyzvzyh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gxrzeyjt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hmezzagw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omgmqznm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2iyqbkjtq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yhuvbhtv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kynfwciy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wafowmzy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqyqqndt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ggfhzfrx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pvsqqdbm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mozggmbg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ytghiadu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hefaazin.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2yuojwltu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2auczxkks.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dsuktlsk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lwxwhbkr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yduzxpkx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hvoilzss.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jqiuzmgd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2vorjekuo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ennbzuyn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lukalwnn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zrblqhin.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2rvsriiyn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2bjewzhrf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uuujkidx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2itmplpfo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfvaikpw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zrkghdpp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rbujsyip.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2utvnzoau.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2myidavdi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ilzczqqe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ccinmjhb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xzpyoxnr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2umszncws.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hufarhyh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2thmqlcpv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bhyxwsya.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kllbdpji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npdsoqdt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vxeikeop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqzfvjwc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tmobnonu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ihsnuskp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpkfbbcd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2scdrhuql.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kioyneff.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yylqfvgs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2rxfdsdbv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2knnlpouf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2unzgtkvo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ncpjdayj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tjwkgltv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wiofoaek.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ftfvjaco.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tefkfyai.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2irfhpwzz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kobfkkhp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mqwmpwdm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mcxpouch.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2gglpbdyp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2avmvbmsf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jzcvgxqa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etaipcvl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wjuergyi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2epuasyyh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cjnwfyqz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dqvaznix.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kssvttgp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xejjhudv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pgteahnm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zldnqknk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zvtgizzr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2obrpivmz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdstjixs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jbogmuus.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2advksnqp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2auwivayf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hbmlycmi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2feadcsev.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qtzflhab.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vadenuff.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwipzshq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhvksbrd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wldiobqj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2widnjkhf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2uuyzuliw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mobqmjzi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rmgmwaij.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqwhspzc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rqnmuogy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bbdmifks.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2krzecaov.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rojllhgq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nmxunogw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2gurisihh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pwkmbnlw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nlpukwii.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xqmpxxsl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqvhjjgj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzokpgal.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zekuqiek.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2omwomwmx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fdzjiaxy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuapuzyy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jbikmwcy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2neeatmyd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2druyhiff.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kpdytzxh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2blkfcbvm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2faojwitx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vfvklqsm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2aategrlo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kmfavwgr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2coiwcesd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfihrnpr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xabejpkn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkwaesdv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vzydtrdi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsttkfmh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ysnxvnpa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hvuebzod.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2juzwqcce.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ixjkdwrt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kqpmiape.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mshbvzox.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cvltmqbd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lcrhmhll.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bblhdktd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2plzuynrq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gkqqhllx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxowufbn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2enllkkbd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2boemeiut.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dhzvmixq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2icfojfpc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ljaudnuy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymfhumro.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tateqfem.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ukzqlfmj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wtemcqol.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohvxjuod.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dolkgvux.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2xzeytimq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjqcydxk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nckybhlc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xnvmiwea.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gtihzewt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qhvrfrum.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2cqbszzyu.html


<!-- 参考信息 -->