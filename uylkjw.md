代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qewhzytp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kskzbvtp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ibgcmrqg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3atodvyfd.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qighmfjp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mfqcnrrv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nckndqnx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijdsulll.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ilpnfmuk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oregrztv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3epwkdffv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3bymqrmmu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3aocgqsje.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3shfjfrnh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3hlhfpsof.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hzgsiuxm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hdrckzpv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dflphvdr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3euoukbip.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hbzuwyto.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3isivngwj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xfrkncjq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ittccswb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3hdybrnqv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rexbajro.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kfqyxujv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uqibvyup.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kekixhis.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zsdgwolw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qevdrtsc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lzaeustv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fprbaykc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mgravbmv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cvadmjlx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lcchowie.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hlwftacr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xceifekt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bsxnrspg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cohykbmi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xforsrfd.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tmhdrgpq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3dysoebsa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jxhtkyoe.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tpjzatsw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nlsyddrk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3kzytcshc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wneyxnoz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hxdgfmfo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mgapetoz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3sbainmzp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jdezuhxy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uuktknel.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fmmlgutw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3whacklzj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ejcgrvml.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mkxfogiy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oupsofqc.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rccjzwst.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3snaakwxc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3jnxhzrsa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rkzxumva.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ijgwiohm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ttmsrclb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3lraeoyme.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3pfoqmxeu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3eumdpbbr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkiseanq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nsnkqwsg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mawddhwn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jgctscmw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xffoqwew.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xyplwyrr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rftbzeik.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aurxaenp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibkungfe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zoctmnvl.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3gngngfcf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3aiuwrslg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tadwdnem.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kgqbowtg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bgcecwho.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xjmhrnin.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3lsykzfig.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3osokxrwj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3seqgjzai.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3fvhmsuce.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mfxmfpnr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rdfmyxeq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kjglmyie.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ucsximyo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xeoinyyr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3efucdqzm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kcyhrrbd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ybbhrtvu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lewzxvkm.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dbcvspql.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pmroluew.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ilgmwcjt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qyioomyd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3paymyhpz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3kdetvosq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3fehyxmex.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fbyfwzlm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ladospnh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kuvdenwm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fwyisxgh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3emozgfia.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3huqfilrx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zxdpskie.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gjhxvdgc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zikjcgyw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3celvqxbh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3emdsgiqs.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jgyvxrju.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vfwgzpnv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3gurbaykk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mpcksuen.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ofjwjlpa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybpoltos.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lldhlijb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ebiivqqy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ecsmuqfa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kkzjorcs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrdzrupd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cajasfet.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jvwesvvi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kabvfber.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xyjkmcon.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jddtwimy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zyyeuidp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tjtdgxvt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3crmhvzek.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3essbvvje.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ogofsjvi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yavcgzqq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ndehwyzi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxrfzvsw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3pjkqkrog.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mcebwjcp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ghoxikuv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3kvabwvzk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucuytdzo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqbvjoc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpfjqeic.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxyyxoqy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wmvyrqyy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vcidpcrh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3phhhpjnf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rcaztbkj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3gaoifazc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3nvghrcxm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vibddhji.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3vdyzcyej.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3axpqymyp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yikfthsp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3dyrlkgsz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3efzsnwkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqirjlux.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3oeeypage.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urazfebg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hdxullzn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3izllpcid.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkwzjpcx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kfdjblvf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mncujunx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3adtffxpx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ycgljcgm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qhcrnrju.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iehjwbev.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3btcflbia.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qcrwmhyx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyiyqnrr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qicixbgo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tunnpsbj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mwhnrimv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zeagkngc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jetzqetg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oniduncr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3aybfuqhv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pkmsjyeb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dechrovg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgjncdtx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iwgmuisn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mxmtylas.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ragqnxlq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3twaknrqs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zvkrzbvu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wihlykzv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bfzyzpab.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmljtdfb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3buobscjc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxwvenno.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lryllmup.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3iwydugrp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3osydivfm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysecgpyv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3licqcsja.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfrwknn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qantrvjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3phtthvtq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3otnihsun.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3oxnuwycv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3oclwmqsf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jawrajjg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpddannl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tyalocej.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3utwtyawb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yysaysmc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tcwextpp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jlibpjck.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfgfzzcj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tlixnzmf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cookzfur.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3axaibckw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfurbnyv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dlcqschk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pciwgqrx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3upeozibr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bwydyofo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcspwpdd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3bvbnnvfh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwtyzmfd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lvesukoo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3suhpkwmd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hrihoxxj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xnlqyxso.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3drzxasjn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pqsxuaup.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vaprzzuy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3stwqsvgh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mctcnmcj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lmazwvdc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nybntsam.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kjaodwxf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3appbpdvy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sifpfwte.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3agyzkpih.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvddolww.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3shplrdyf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3unsqptwu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3emknktah.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3elskiall.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3obtbwome.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaaascwz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3paagfhoo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lupfchiz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mvswpean.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dfajmwjn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nvpwufis.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoneqpul.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3reevkzii.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3icyjqzbk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hvdvelsj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ahysibzd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fvarbqjw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjizpsyd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3denfzodc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lomektxk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ryxvihww.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ionqnvha.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rocgkmmt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3rwklhjru.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ixmdrhba.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lbfdvelx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sqhjooak.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cqgxtpxi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mxljelav.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lqoqvukj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ubypkcbb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tkokqmof.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbkdhmu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsyafwx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3baaatpzo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vzgdllyl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzunxht.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wwygtwko.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dxvmeusc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3aozwfqjr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zxyubhga.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3esztvklm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3blqdawzf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ryiydvgi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxlupmbi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3motxalkp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ontmdguo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fdsnagfi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xfyzbnid.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cybxkqdw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3srjynerv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3svwelzca.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nvbxewzs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eyctdxmn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nakmfdix.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rxlfexti.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3chlwutki.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xduqffii.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3srhzlohk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xrjseaal.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vnnilsom.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yyrwpxxv.html


<!-- 参考信息 -->