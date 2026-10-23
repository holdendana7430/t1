代发 wailian999

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3dfeswzdw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3khsrdprw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3hgjztduk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3feanmuil.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtvxkcq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nehnjotw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fsopvctf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vlnjnagi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3serlqqfh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3zbtghbdg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sjjkmawe.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dnftdezy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfenmsbc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vjwatqyi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qocufyei.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nyguaoop.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rywatgeq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ydpawvlq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ruahfxgs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jphllefj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rarxznhg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3mujguyyl.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3pfmnckyt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ouahjlvm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hccouuus.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qogewsuj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mplkzanh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vyfockuj.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3nealagpb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3yejppgjk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wmjkjkmv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3likopgjw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pipuwpbn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zxmsxhmv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ayudrzks.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3aezrxpto.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zrlqttls.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jhibwrpg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3etpepzam.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ijredcyc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ehdvilig.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vaakjqkr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wsfizmsf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lfoptksc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ywpbxcoj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3figbkwuf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3aywzlqtp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3tezxcnmd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dvkcxpch.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3noxbkweh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ubxmcbzc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pcaneufc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aiqospgq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nnyexydl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ewqnscmi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3psjaprup.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3dbxsxtuk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xfdvvnmq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3exhdkbqj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3neefsgtz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3khinisxn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pafqrgat.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fmmvjuip.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3uyyndqod.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mxdgptox.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3munfapvu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yzpyccmw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ihufhvmo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ovreuyxa.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ufyeydif.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3nxqcumfu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3bxukpgtb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3iabawisr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oayccbji.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3igcrwryl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3evlmgqrv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rfuyzdgb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3waprhafo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3fbtrjlwt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3tmspxqup.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3odflziep.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3owycymgf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uniiwehr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3xknljdft.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3azepxmwf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3shntrcdp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3msztmncf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nrzuwevl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnulgtmy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zhfpekzh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wactqhzd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zbsvtaka.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3zygwmzly.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xzcwonav.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxhdbvv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kcevohnb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gheqzhvu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mdxmmzzu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3pcvuybne.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3imgnolze.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ssztpkgv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3xfzxlcbx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nllygtty.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vifcammd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rtljhukx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cuscupwy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3yjlycdjb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bqxgudhz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zhzwxmqy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3nnvbxxus.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3zrilxmif.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3svlylgwg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bptnnbiw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3aknxabir.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xwljaigs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3dlimrcsl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3bnflpqvu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qfknolpt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fcgflejf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3arybkcbv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmvxdzfg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3emrumfxc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mvtffxpk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wybrfowo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vquetbrd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kwznwhtc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dkawkele.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ykhgcrct.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uztnitzh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vduvcsid.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3uyineepr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tswuxweh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fxizvnpt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3igvalkra.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3cwuzpmis.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tslhhmsd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rgxmnwiy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tlbitagj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qvhbywke.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ydcecnly.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zjrfksiu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fbdkqgdi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wndefedz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xbqztqdp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mthxvyav.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ptalutif.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ckelajms.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pienayyp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzylyhok.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vfscqmwi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jzfrytcl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3dordpenh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3aoyqwrhy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3htlxqput.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iaapzmrb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vhillnky.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zrwtuhdd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ejgfkaso.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkaxsal.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zacvsjjn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3urraelmj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fzgdffql.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hwdiahcc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpgqthdn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3fecdimad.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3skkhgjhu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tnarzpgi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3quabuwzi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rfqxxnyv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mmopjbda.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wrqewkjv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3egbmlfkr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vsccbpwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtpdnrzp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3aqzbznpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gujfpctt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3usfcrmmk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3dqartvzj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hysqhpfk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dmlybftk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3evmsvxzi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kktllzxa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3exgvhnvz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xntpllkh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nlsubisn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3tsrkfchs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3kiyiegmm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptrynadk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aidwnwpw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lvhlvnjx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wxazsnls.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qbdlrpky.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ihgzwcvr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qqgsltth.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vjcrmakv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qgpqapoq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkliboqi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbkgpuqm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xueyvmar.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ngyrydcz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tnldvvqy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vfprrexm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hqzehwon.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hisdeafd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qjodithf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjrsaxf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbnqjcjt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ouwvkkvi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcownugn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zdrgfzam.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mgjqxipf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qntnzaix.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ssemoejm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pthhelaf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3uqtghskg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zrgprqel.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxaqagdv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3sotcqqld.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3etsdznyg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3nucaziax.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ahnxdkjv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ywxfdqpx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3imbcytsy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqhatdp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zgrzvkuu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fgrlhwoc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3zxzkscxo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3eiabttkw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gmembcvn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckrawyes.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rnqxaeyf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdbfpxut.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lrgvybce.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3orwilejv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsidhlrx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jfhosmgo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dfefxfhm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qgqbjkfw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dkhiifqr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fuoeppid.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kbrnxdib.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3finuretb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jphpitrd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fiqwvlor.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qgjgyqru.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvjytdh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3euhmergm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ccwnigsd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3rxzxdqib.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nuqvckba.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3upfthgic.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nzmgctkq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddfwclss.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqfkptbj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yieqgftv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxnvkpsj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnqevppq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ohtfbcok.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wzrjwkge.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3holvuasj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xhkcowyn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sdlwdpfx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dggomlyf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtvjspi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jrtycjuw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3azkoqxaf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3njxqhncd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3toaakkgx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yxbhwyes.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mcxbmgug.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tohpfgqm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3brclksqv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3uwiqthnq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rbcaymlk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3prwbekyc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3piqjrrjz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3nussqipf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yryahnju.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jrvwzxfm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ywyhopge.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vckzqfdo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3iflrchgj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xdiatbch.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uybwqkom.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jdfmbzee.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dgdcwbhp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ykxevgjb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kykofzwj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlokojky.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ahsmcwln.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wfujakpy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wqbfikae.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dnbdxtpk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3oejisrpz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tvcqtapm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fjriengu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ktxuzqqk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bahqjvcu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ikynvrzd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lurpjfyc.html


<!-- 参考信息 -->