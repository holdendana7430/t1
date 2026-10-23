代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wtzuegju.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3noyocauq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ncadrtdr.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3wtzfsutc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlmvjqc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pzrgbicg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ygxohtdf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gnomimxd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qxppgswg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bedayswm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wvmfwfdn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3jtuiqapd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rzjkjfqh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rriwievz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qsexefwx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zrbhsnpo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3owmbytdk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3swieoqow.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3htqywfwr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3hodpfvcz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3eqbhxrya.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3zrkwnbkx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3zobviypo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fixbsifq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ssqffxqy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rfsesnqq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zespgoyw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mdplerdc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vdupatyg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rdefolfn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebapfwza.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oryzyumu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3axcyhqqp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3tyikfrzz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ivcyuclz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dmeexdys.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3inheasiv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3kwgmifrz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ecwobtdv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jdjsvqvn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3buuafjea.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3hmundjou.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rxfqnzqc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ycpayfww.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uvokwvim.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yrdgxhmd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3yckmtubw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3mobmuhqd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nyguzwdo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jtfupfki.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3swdbblqv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lrkkwnkz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tdstffdk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rcxngbpc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urwuxzya.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3tbpxcaaa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3pakrymzm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3alhsgkpm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gnusrikc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rbaomolq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mggysdxj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tckahbay.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xwbwjqfu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cdsnrbrs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oropmusm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uvhmwxyv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3imqtvbym.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqqfxxpb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vziusnmm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nsimcigq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tqtsvplv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kipqpsrp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfzsmrl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3uyvbonjh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3cjyxbolv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xozhzsmr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hvbgwwdl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3vlykojqh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3paybnbso.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3orokcilx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lozcveyd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hbvqojpl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ajpsrjzw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3woqeyxer.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zeazzgie.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3mvzwdcdc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3eohknzba.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3zzuhxgfm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3scjkqibn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ofjccjzz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jqtnewms.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3mvyosley.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tibmltls.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3reazyfrj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3acrlerzv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3anpbgwlm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dpvokbac.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hejmihyi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dwlarxrp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqydhxb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3chlaadee.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkzkqzi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pvmunity.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3udnhmiqi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vbrjihaa.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mgukowxx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3fkvfafbj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3nrzvtjou.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3myniqqfg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bcnwknrk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3umrbauox.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ioefdqci.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3oaqfmgjw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cgxtcnbp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wkcdisng.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vtrxncfj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vqhymjvx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tevvpjqz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sczoeqzu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upyotvhq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cfhjriqo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3nagnmqlq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3nebhioeo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wotvbarz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3porwgefp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zrtymwjp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yptufczw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ahcoukam.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cbdxegpw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3qufuugst.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3aqnczaoz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gzscykvl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3dqvcywxn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3iftnyccm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xnfshjun.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yadgtnsl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujxgsuyj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zmxdcbyr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ahrprivv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lmyoummw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ykrkauef.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tillqgwl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3oalcmnax.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vzaiyrkz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3utugbqyr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rcmzqitl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nuzrxagt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3umxhisrb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lqrjpoqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eisygnxm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dvicozgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmbgpcqp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ljypldtm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3uszxhcsj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trtoosan.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vupmdmqb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kzjtlsqr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vnbtfkun.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3hbguisjx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3anjlmvbt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ldkuuyyz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cwsyxzvn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zeorkqyv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xveshlgk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kpyypiyr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yxnvktni.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wiwewrxl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qmbltmzx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3flyujuxy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lovowlao.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3brolnrku.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3dsyzhqur.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecrxgebd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mpagpoai.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xukwhkou.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lfxuowno.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nlqthrks.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lnlazcdo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tlksaask.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3oobydkpl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dprbygbn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysqueham.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozrnxoqr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nldihpfy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldjpzmgh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cpkgzwcy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3sdyfsxta.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3iyxlidhs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ikikguml.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jzoxirnu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wgknayck.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lybhqfmb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjqrgujk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3weflqgnb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxadegwj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ccbweocb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rklwvroc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3eiybxkkc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oqfdbwdh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3athtqdhr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rruvdimb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nlcxcssv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vffpvtha.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tyglffym.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qwgjfgqh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3givabyiz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wvzppdqt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wviuaxpp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3szhjfpie.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lyffodon.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfhekoui.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ftxgoggu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pbasiygy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ryohhdkf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vxogvbku.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yaiaoitz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mxhuouhq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yjwrulos.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jbpkfwjk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xxftnhpa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nqjzhdsq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ynjgytec.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3eknzxpet.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hkuvpjsf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3clwpjami.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3apdfsfgo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wbyyqtzu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgwvyzcv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wohxadjo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmowbpkk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pblznekp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhlqtwo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxubdsae.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3liznwxkm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrejmky.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsrpwvul.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3efgwkjjb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jrzdqkdd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3itkorbac.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pjqnlloj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3svkqmsqh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3miprddun.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xiqpnlgl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3gntxvsxr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dvvpuncx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kgscymmk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rnnsyfxo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bmdtmbuu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bgjrgywg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3enyfwvww.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uerkphjd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ityezfjw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rckvyxbt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mcswqwfj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3npscozgn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pkomabzq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zjyzlfpm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hlwzqbar.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ihwrkncf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fvorcvbg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nkecrtzh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nwhgjdif.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnoeznfx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3amzggilu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3namdvyyj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sgofypmd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3uvnxmsxc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3evtlqysd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kihitsmw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3atcuoacd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fddiojmt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3aiijpgae.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mvckqumj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjijanua.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwfwbhli.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3swuaovac.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3orqvtwct.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzlffxtp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3dlfnohns.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3obtnmmwl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xlsynkdb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ugnvkibb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fxaetiad.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3weuvepmv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ouowcsay.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vkrganjc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pbvwduud.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kjauxylh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xjmzjril.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxyiwwbg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jpyveblp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lfgvcqrm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lcsyjmwp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iryjcbpa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3aygalvbm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nxelladz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffptrsrj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vkumisxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnbjkzwo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mymeykhc.html


<!-- 参考信息 -->