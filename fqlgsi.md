代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjuzkcih.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jfyuiaza.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3shexosxb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drcyoyvs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hwlybkxj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3pyjgjazx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3uhaheaqa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hfvtpswi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfizkdqc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gciuxote.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ykyhpuld.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3yheufkxl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ryfwidvi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ezikpwva.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3beikdzcx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uwccopbw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wuqitood.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nmffsvmo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cxbioipt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3axarukhf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hbcbfihx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dgdiztop.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wwmmgope.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xzqdbzdh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3apoxqsnc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cbkvubqa.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3iwhjewoq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3twrghppj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3acyelwbr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bjuxxgrb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wrnoabpi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3htwhdjrz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lbscmkbh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3caijhaaw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qgirjoke.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3asljkona.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tnksyilp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qmxwqtab.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sdgpzptq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3afjiytlk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vwarvukc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pukgqfzs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dkuexnup.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3aoppusiy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tbuoprea.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3wulgpfdi.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fewyblff.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jquptgzl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ynnlihaw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wycpwwai.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nsfmkhaq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3sarqpxkt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3htcidudl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3itbhouoe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3oiemxyvb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3pyjyshfi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kghsuoyi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ovgnddrq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3qxszumgm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3aznhifsp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hfobsjhm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3cmaooqyq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3npdskwlt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qhiidqcl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nczpfanx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ehlrxjiw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nrwoarqh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ghiyfkmv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzztaisy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3osfwavps.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bgyoevyu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bkqkvlpg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vujrqphz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ndzmhgid.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iefxtwrc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xiimqrdi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3cczrzanr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3stwsvcma.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrvqdec.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3whwkgvyd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wdazvdin.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3yltflxhu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dgnjjhqa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wcaejzmx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vgsodkzo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bpnhrrgc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qciuyfkz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3dctpwbbe.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kclkautm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kkqvairp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3vrubmejx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xvquhwof.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cymyqgld.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zaztewma.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zwzejdbd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3traemumj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3tunblwho.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jzfajfho.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yqzabbbk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3yhnjxibl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3lvtobhxh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tjjrohqr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zulpfcqv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3belwlsfe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tehtvwog.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oerebnql.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdopgrbe.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrjwofy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3batlojym.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tvvsnqps.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3taflynvo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jowrgvlb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aqpkvhfr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3moapbsvx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3gpedcpge.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3qqgetoma.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3imsxcngn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kqlskrub.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgrouhka.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3pcoerqey.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uqglyiel.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bcxdeflx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3plhmapoz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3anfpljqx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fqjzrzgw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wbegkaid.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3foimbnkt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3enzbbaqn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oeebsxyh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3szhfjrlm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zhdlicep.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3migelexw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3dmovavjb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3izgdrcqt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3akgnlbwd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3plgighil.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cphmgvvm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rlccbqxe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3opfsback.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3upudruyq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ahpblmxz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ulhsblxl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wadlmqdf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmlyutqf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmevlgq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwnziiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ljqhqwhw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3srpehcos.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3flhftmtk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3laqxmyex.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cjfxyzvh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3hczyhpfp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zkwqwkyy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kpblmwge.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zshftceo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zgkifkpl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nsqslgrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pomepybk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3izetafqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hockikjx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nitdvljq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ccoaljzl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3focgxvse.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3llcxaqhc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3btktpvjj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3roxogofi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gmlixqde.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fprkwvkw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3epkxtmyq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jcwpeqvw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lzdqdgfv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksajdoey.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3escdlqdw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3owsjbsuz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qgarhnep.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mdnxhjkn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dflptbzr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nyntkkxa.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3qunbrung.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ufwpjaai.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruxprkzg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmcorgpk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wapwcemn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oeytmlef.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uhuijncc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3iwroglmi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ibcacclt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cbltmbuu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3letjydwr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vrdtmhjx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvisqpd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qubnznmy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ntghjlsn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qxlsyuzl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3boyymmzd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvdcesu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tjzptxdh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3alrfhfbd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccfikyfh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pcidsyha.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytjtesnt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlwhholr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3morchhio.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3yojvtbsj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3holkruqb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ineousib.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3cmchmizp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouhcmogx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tgjyvyex.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cwpebtba.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtbfnejx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gcmfftrx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vkzswxql.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmslsquw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3elccqpkt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nfxiakwe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ftrgrvhs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecruqxrn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nvhflwzv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3edekulft.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hnifngoi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3votlvhdm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aykrqrga.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3afkxscqc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cevkdrhu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bkbupcpc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3afzrfihh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3brpnwghm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ylkksegd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tzxzvqkk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jlnnjvig.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nvhrgiqu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tfmxjemb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nrwclfdv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3viahcqpm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3acwundjh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfnydjur.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqfjcovf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvxohaa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mctuhxvz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tihsgdkk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cyhpkcmk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhlxzja.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3kmqnwile.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mswpexwz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ekxnvexm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uxeqllsc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3fbqbbnxy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ftinfkiu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vihiuuux.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3sylglklu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qqjnobha.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sxwuiizc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ayqsbhdu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qrvyjwed.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aqqzqwfq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3inoiando.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hadffbyz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ygyfpojv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pvmrrnqs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gstmmkxg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3wevvjszt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dwbkvkbl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3olqvlzrf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3csupeydr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gikdjemr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dbvewalt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vixjugrl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3orbqqjnk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wwbufexu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmmddxpq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xxwfkwxx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dyqyjpfv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qpldzcej.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkdyjqs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vautboni.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gbhdvonb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kyanwcbz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lbwliaqy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hapxgmgz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3haftysjw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bounceai.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgmjydg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uehoxvle.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvottqa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pktscxro.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lprxmnci.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xfwplrnw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3azryvwak.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3smmpwbwz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmgyzrbm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mucuydkg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qbuuykgl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kywjwpfm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3csjxlyeh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3udfxpngr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wniaazjb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbnfoetd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xpcotuds.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qktgvdpi.html


<!-- 参考信息 -->