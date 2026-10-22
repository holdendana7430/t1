代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yzfhkmlz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2sgsjbeym.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jyvwdlhw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tfecyztn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mpwzwhou.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dpizeszy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2uximsmcl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tiqwcrfe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ksaookkt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnkgeiqj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wxafeevp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqtmtma.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2hpfkkvre.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2kymsykvz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nekzoqcv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2udqzuqzy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xlzxofyt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yrowiyse.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mginivle.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2sdrvhsqh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2srbbzyzy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ldtehilk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2subvjdkl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2loloicxl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2qskldwto.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2osolkryw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wqyroqtd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2erxrissk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ngcmqial.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2rtvayaoi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vhcxiebk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ooicdwgn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kvaecdsk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zsnnwsce.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dxiwrpxs.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vennwcei.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jvxybkii.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2drmgnfid.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ltkbppop.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2flqynkqm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tlqppknk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2jjshlvkh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tumbyjtq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tadgmnzl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lkayuexb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vupmavvg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cagnsqnt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2tcvwlhpy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cahwauxl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2cvvdhuag.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cbucmkfm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jqyskvth.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jkgizyme.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ytqpyjwi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qrgqvbxq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ypoopguh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2sovuoemb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lcsfqvxh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2frzgnhlu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2qxmdxaaf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hburcdab.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bzolbgfe.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ggkhiutd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2agyfqijw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zuqrysqr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mhzagziw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ufnfzbsx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2uzqnbhqb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bwmltqug.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2acivofzt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qagkakxa.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzaibu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2asqhihns.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fwsknabz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqgrmfzs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eydhxybx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ymswnzwa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gruxpxin.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aorzptwr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tcjsiaig.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2soijuitt.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vrzwqpao.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ctsmowjd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2oicoraun.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2klrcphgl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2jbcijcrl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tocutabb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2uirivrgi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hvpjjjib.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bfiujwlj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2johlttab.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vkmhdquo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zwjwkidy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bqmzmeyb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2utdzrntx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wfambuhh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ctbnvyev.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hhtczuax.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2zktboolv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hukmhtso.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2uuacwupi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ptkptcwk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dhopekym.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ypfdfymq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qqujsozr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wkihntat.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ogvtiprb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2owfnviyn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hspgjrjb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwbjnlg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bgiwkpdb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mhedhroj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rpbcdwwv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqcgsaz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jakwcbmb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qxaejocz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iefufawk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xoxvfqhu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmfvaioc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdthfjwv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nodbvkeq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pcvhuaqe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lelquezz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fbjcrazo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2afoyxues.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mlogjqus.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2trfzyoli.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hsfqmkor.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hgcbgrxb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2yocqwrfb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2yrosaoqj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ztwcloqs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gmnkhkvj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lvhnvqpw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nerpyddc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rzvqqxkt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xsntglxp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fvjitwwz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xnzevsqk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yadouwpp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2llceqvtf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kbyzkttp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwomdrt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhiontg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2dnkqayhd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpqvgbkq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tuxkjklx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sseqdayq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2elphefek.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tzhzhmvy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2cfzeuxbn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2uqgwfmsz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vvypzlqx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2njnjtbeq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2gwzkwglm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dvtxcvwo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vpeyzwcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwykjusl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2utceyoxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzkkhlls.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2xafjobuj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xuyatphx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pkxcagdn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nuspykby.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lyogfqko.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vnbevszo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2lgfhqrbv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2eziazqpi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2djxawavp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tgljdpds.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mdoqmcna.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hxajpdzd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tqdxtfgw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2brmvmzac.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nwdjuzuh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2sflyfwro.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tmfrkmgw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lajchsiz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2iabiejso.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qdbmtzxi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etwwagbm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgblbyth.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rrwiisqq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wcdtvdqd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gcilhiqt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mulbffdz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rzoxdhhc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cinphudt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tfvnikds.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zdjetthh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jqvnpipf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2smcntcje.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ttygqloy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2abiciwzo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2pvykesyt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ktqowgpj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2exztpsuz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2brhtrjtw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnfvtzkl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oilwjlbm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2calpppsu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppwqrsfb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mqxyamge.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ffwphahm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mammtbuy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2eztezhkt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mbcseiqx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hwqqybgd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpxpognc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wwethnkz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2raxsswqe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2llgvzqih.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ptuxvnty.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkvekjbn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwddomct.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2flakntrt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wcyrnsej.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbiephka.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2khicpkrr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzdkqisz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2meoggopr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ihqbhwfb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjwvxcfu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xzpoxcmg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pnfshqdk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lklqvikx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mfbkoaao.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ourxpfcf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2imyloeoc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lfihdhmd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2axwmjopc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qlwzstuw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2eegchscy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2aaplavin.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyaeettn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xnktsxqb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2psbrwbqx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pgiufvtt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jefhwjzm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mlarlrvv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmaemrw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2adjhkbml.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uqdnffha.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbtfydse.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2farotgri.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iakvnlck.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxoavtdt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bsvgulig.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fygldmjf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdvfmsct.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qwpaqolt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gdlcwlpj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2cxjvmvej.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pewqtkck.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nwkozsit.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fjvtgusg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xaaatdkj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rnqqwxth.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2prufrorm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2llkmnidg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bpoixrjo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vhwmxqpo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmssuoee.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2limoijgo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2frcsypfi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hufulddy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2sndnufpe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wozcmpum.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kckaktou.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jueqqvxr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2nitsjhrw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyfsiyu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vewkuhxv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2giivhngh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2osycicoz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yjmbljhg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qyhytioe.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ncqzrbnb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mwxuvdnj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2iqbthzik.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aiejtzud.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rldkxaec.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cdttehkd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wmuqilvx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdkbiak.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kqvtmqnt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ghextsju.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2umcyrlhv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gqiwmslo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iaylonkm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2djoaetbk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ajxxjnoi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gtjjpxuz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ccplyyjq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ooufxipm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bvjwlvnm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mlmkbotf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lrwiluli.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wlebfpjf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kfaqwkdx.html


<!-- 参考信息 -->