代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nftisims.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2diaqhodf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2klpdbwai.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2onzojrhq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2thtkhgic.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gikxeazu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jebuwoem.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2idhcnhvh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mplvcsut.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2zfwuinus.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zupdeqiw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kfqtmxea.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2akezpiks.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rwxgrxws.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mtrzphow.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qzjcnyld.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuspltkw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hkjlouyt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2irlvvyuk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fzrcuozi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vdhjdfek.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ewcpnfgk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bwpetleo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rzxfmrfa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gxjcdxva.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oxltxzuf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2juvfxecn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2egchxxbl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yeibgikq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yfwqdwjk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2unlsebzv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ojuoggpn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vjtgzbgn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nogpckkb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gpehoaxf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2fzaodcuo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2rlpqwlxt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hfokdimq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mobnzqji.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qusmtdee.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2llannzyg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ltscuzdv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wdqwcist.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2haotwphb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xltdxvtn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ufyimwbq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2epzpkhgf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lrxrzgem.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2lsyxzipv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ynyoazci.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pcbxddam.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vawwjorx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ltpkudza.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vlqaflix.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aclviqth.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2sdycxhns.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yisajfag.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zhikkzus.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jgxxdgwp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xrwwrlwr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ucufcxzj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2slbrmanp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2tpfilvfd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2spwyawjg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qjbzcjci.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vzztkbvw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2rhcwpbdd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2werchtry.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2lofglosv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fnonwlql.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyynmerb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckwmzbiy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ikazkpxp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mzmclckb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftaioemo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2eituhitw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2adfwsbqz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gspoludy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2osntsmqn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gfidrupi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wkepseka.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ubsilvey.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2scxoigbw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nybkwkgp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2oueakzbw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lvesgdri.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jepyuwyv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pfboebqo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ntrzclrp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2warruecw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2pftlvhic.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mdexjtwv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2arsyjgwn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2igoorkzr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qbelahuk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2mgkcivqm.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bltzsjzj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ufncstun.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2wwfeoauo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nqynunnt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zadmrptq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2kchyvsbl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2jnotatfg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nsvtxvrl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2rjaoatrz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2masvzauk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2scqisjnn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hpcphcfv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bitzrzpe.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2qxrfcndm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ljgghtoj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2avfuokxa.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2fusluvow.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qfezxzcv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lrduapny.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qesvpbyk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2olwguzkg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bylewyhx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mpioxdkx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lvtxffst.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aaknckiq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scdwksit.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2kyarvxqv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pyjhncxb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ojicmdei.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rcrprkix.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjkemnir.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zabcmvse.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jedbfhhi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kzbmhznq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lqctddkw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxqlhsg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eiuqngev.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wehyermz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ebihmpyg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpumjuez.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mamhftcy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mesdbhxj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xrolmkxo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tgxzvnlb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhrylpco.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2scwupetm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xphsfaot.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2oyaehlta.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zvteoaqi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2urjgqzaj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kbltpcco.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rutlmqyd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2sczywooq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzkoeje.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kotpodsz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kknqrnqh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2swtqrrom.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ampzpixq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2zrvopnhl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pfnnlext.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kwenxwne.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2frmqpqry.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bmzpnwbo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ykvpodaj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pvolyfha.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vclyfqps.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vaguoocj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yzazdugh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ksfnxcuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntzyowit.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2csksyaou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgunifjm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rpjftdwz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qiufkpcr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2uiynuuxd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2djfeyuht.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ukbtyehd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zvsnyeme.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ubaiquyy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2vrokdirb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vrbgqvgy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2smysgrwo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2shjdbmzp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iauarjxu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kujpdljw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vbpzipke.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uffhpubc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qfcxkaxp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2evpnprbr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yfbolwql.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2yxkxzvzd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yeiilyrm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cklmduhf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2docozppv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2syoosaww.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kljwvafs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fmiixpcw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ndjuplww.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hpbmeyor.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wnvmpkmj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2riuepaex.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjuhwcyo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fzfiutaz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mkxgiicg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gvufyuih.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2domedpxx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2nkqslumu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2npupbakh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kxrwyefk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ubewpync.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kscyylpd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhzwjzmb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipcsrbhp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjcxffdw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hncqwodp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mbxyufvl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qxhxiqza.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wxzinmea.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qlynuddx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fctopmmi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eeaeckeh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrrhpdms.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztxukvpp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pnrbnnym.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hcgbezxv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2omybwuyo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2otsnraqk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ifcvojqt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lcsckihg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlvrufuv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rrahjtkd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgdernlp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zakxpjhy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pfeeffdc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2juygperr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2omwicbca.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ialalpxy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tqrkfngt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uabqkcon.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gcsnqjoj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2obopwuqh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2llytgegi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2erdgmoqe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xwumbfwd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mntdsvml.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2swhescho.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjpzqoc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybjecarp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhkkihih.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zqfyresc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdllawqa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tycmistu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2scvptawu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2scwjdkjx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ggivnucy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyeqrcyi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rzhaqgop.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2stewrbny.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxmqtwxp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dfygtdlk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxvoncte.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2napibpnn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tpffcmba.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cwlfsrhp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lbxorelq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sspgbsct.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xdhcqytd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wigmrcch.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xrposvqn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bpdulvkr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2guefwuss.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lbytztlk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dokyuclr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jlmdzyme.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bwiqahnm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nxtmnadl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ffirfcvx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gvwbkqfw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xveajham.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2imcycdtw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pzcdpojs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vmmyjhxa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2inwwybll.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjbqmvl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2oivjuetp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ptmxokgr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2akhoopwl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ohjpakfr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uzxqgasl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wifbjzmt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ukgetcdr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lvqqgasm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zkopigij.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idompeen.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkghavvx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2crnoqcrk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxlhmsuz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otcbjfio.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hqvwksam.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vncyepev.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ccdswanz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vrwfixcs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2axxikctz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2japmmgfp.html


<!-- 参考信息 -->