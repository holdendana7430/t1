代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bozxzkdh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mgpuwftz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fkycfbhh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2szyoxmcr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lxtieyep.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjnjopuc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wetwfmgd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vkdyezcu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sguvaspi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fumdfszx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cfkhzvug.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lihkflbn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yptmjymw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2yhekssxf.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tppsyucs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qiqjeehc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2delsegxt.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lmjfixtr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mihvmyfb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2uppqtiis.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2xukvvtzz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wacijytw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2illxbuib.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2impjacxo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2korfsxqu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sfggmika.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uesnvdyw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pazhhgid.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kkraeagk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pfbmvver.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ehldxlzd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2lyrhuvcw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jxmlioqn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ebgcvjpw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cxtiypgw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2akoumxxz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ctckxgap.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nxsimwkf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ynzdgkxt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kxantgdb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qqytoonc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2blazpghc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2avgaeepi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2blmmzqyr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wfmhyahq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2duvpyadu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pgynabvu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vfclxvwa.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gywsxoio.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2upoxiujt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wqdmvnpk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fmfqzdum.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zwkjyset.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ukqfmzrs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kdlbhgdm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2epqoaqfx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2czntpjfx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2wyfggxdz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jhjcdsrw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vzzxnyfu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gqhjhyqw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ohhsuiro.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2kidmkviz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tkotlocq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ozzdyohp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2biekyqkf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2hgdhnpca.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qwzszxjw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cfbifzlt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2hyouazvx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2vhbdriey.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdkokkkz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2stpjrmua.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kmojxjho.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvdtrici.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yujdgqza.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsdfydco.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xmbjpngl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xsjdxcmq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ijexdthb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rblbvnyr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hmylovme.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nzuzjgce.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xsaecnzo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rmemxvdf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wwdhvmnd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2yrowhfhb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfyhkmy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gzhdbjlv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2sytjmrqu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xgadsyhs.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2evfpjgpp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2oekiacvn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dnezqbex.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oxcpkyym.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2cktlvpks.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mbupdlas.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tjuhzrgb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2xkyxjjlw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gdwhhrvb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mdvybddk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ezcdctuw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lkhobmrp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mqeyuhnu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qxzrgobv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zrmsbqbn.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xvorahmv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ozeqliiz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xadpxzxh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2kodwgvhs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2eiprlaak.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ipawgrth.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ecgwkfia.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rndcqkqc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yrwqdqgj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zokekrce.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dzbahgkz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yvizxlbs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sfwohlkb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xpjjyaaz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2znmpbggf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bqmgbpwy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gbdeeafs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2asfdobpi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2tjudvwso.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wzycjooa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jtahvogd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2toqmvqet.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2inpkfcyo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uwyojquq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jtqlmpqr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2znwvliss.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2klxlhqkp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2drmivffe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mehtvgvb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fgqzzwtg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sygmoacq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wcexjwar.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ssotcqqg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ewowzzes.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kivajarg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wrfygjri.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pduwunlp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wwnanlkj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhwwsyr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mxpfdyse.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pifskefq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xyexfzgr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2pznfdrcp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iutfqtsr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yefzfsxg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bxtuhlea.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2seopkkay.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2khwrdanl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2slodbusp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2khbmuzbj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dqexabxj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cnvenqyu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2tlopyxyi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vbmvuokp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2yejncktl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hiwmwloq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2gqgcywtt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qhfgqhsa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wnmkvdfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsffhfes.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jpxltfoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngclvbsv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2clgdgegj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2sfinhbli.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkaiigcv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mplyhura.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ikklirnk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2npmksjys.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ryavjifn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qcvmsadg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dbxeoyqn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ggbajdpz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tjxhmadf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ayyghgoq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2egoljgvw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yoyqgity.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bomisdnf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bukptqez.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2olijqsne.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dnegbnsm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2rltuawrq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gjspbpff.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dadmcakc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmxseoun.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nkitizul.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqcnuxfh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rzhbtgqs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xoxlaldo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ockjqcyp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uqubpecv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2htsxcadv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2etjjyqyz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2emhjvnvx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vhwirmmh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ajmrowky.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2atxwgftx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uabgamua.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpqemqrp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ijokpdlp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xxpghdui.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggvtjxyu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wybjamzn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qgbkbuxc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocrqlpoq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2curdxday.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tvrkvwwu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qduahiiw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zkkpznyc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2glnopgnc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2asuduakd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fsqrrfmb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuzprpzk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vercbjtr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2camfikci.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jsikjkpy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdtgtczl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yixtqica.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pupiswka.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ojnatkhm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rxdgboki.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2szfxbiun.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2febyzaby.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wwlklbeg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yjkclmzs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yayjbibf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jrnctkbw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2atnfuwff.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2laoddpvr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vfqnqqph.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nkmifgvl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hwsirqsf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zsoxavti.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fanzrhrf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ctipktij.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qbrlmvvu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ntrwxmcb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uxfnhbes.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpmbfxtm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eobwtndj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zswfdpco.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ehnfjrcg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xjrpevnb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zntvicto.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dhkvjskf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2evxsamxz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zlzmmpju.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2koxtpggx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kxzyrsjg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2edxbshtu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kbwgvzgk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ithtqpzk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ermjhqan.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pownrefh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2smglvvpo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rlpevtfw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2podzeubo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2efbkufbq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2whvsaxcd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bellesfv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wrkjbmkd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gufykeyt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tdrwjjuq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jhdfokfq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mmjwusva.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjscuzl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yzllztna.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uvmukfjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbjfjzxn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kpgrikym.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lesabmgs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2owpdjrwv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ddtnoljw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzflulye.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgweouxr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sxibzvsl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wwxyyqaw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vleqnpaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2iepmejmh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2scjpyzmk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vpsjdesz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fxppphiz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lqqulogi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpstqpxt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbobwoo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2taboasxt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2suojqfbs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tewrzbgb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wrehptkr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2lfdihdxc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2klpbkytf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zpyhwitv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lrnnbrkc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qkpmygnn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cnudbaqs.html


<!-- 参考信息 -->