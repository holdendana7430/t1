代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3afxoszhu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hqchayja.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qvmydufh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3rmovrtdk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rgdvfzeb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wjbbekio.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rmnyachg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3iykurcap.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3aieaaaci.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yaovhzio.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gqfomrgd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3qsjuhtgp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlupfwe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qsqqskxw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3upnesotc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wyvjchyo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qcdbvnfh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3csratwhw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ilmzjluf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kngsreht.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ccmbsemk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wubcpufa.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rrldjhbm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3znetydoe.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ovxlifbp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3oaigfpcv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ozivzfrl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qlublggk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zshwcmgr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3sjgyqoyn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eqnsqftq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tunuqzlb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bcyoadmq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pxlnptde.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cxtlescd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kshdodxa.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ljoitkix.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ssvazsha.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ytlbzhhx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3sjcehxnl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3itgwqauy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lrusnqzc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vqwkxnbv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nxjxfdqv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3owouckvn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3dzaazzmp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3bxkypmgp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqkeozvy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3asixmuvo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3utnviall.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jahtdmpa.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3seevyhow.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3khnfzbkp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3edjjbisl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vyhivetq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3maqjyedq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zmgsvbpl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wbjdenjo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pstdamkf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3srmkrsix.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3jacjpmye.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gbqxgblt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3arjwamig.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjnunop.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qrsdakbz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3yvcvxtkh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uuhuicrj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pknarrzt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3oeqidimr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3cgtfzatm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3guxvsjck.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ydzbnazq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gcvdawmu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jwfpskqd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3pfltriuk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eftdxblv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ddtfecse.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lilwvftv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qdhkunrf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vkwzaqjk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3qsmjpqlx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tpvqqrjo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ecvsvdwc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qvfplfpj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ehrxjwfw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qlmedhbh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3zrfccpgf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3uvuidkfy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdkdrisl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gtxiuvaw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3atcacsbr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yrjqqlfw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aawjldkn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3enqluydj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gpvzcjhc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wugdtqtl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3asmlxffi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jvffycar.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3imgvpsvn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rzybxrsf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hkjeesgf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lbsmjjip.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bppsjcaa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3awojjbol.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3npdekfxn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jgyfsark.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3urlvcjra.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vacccdwg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gvjweelm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xgtywvpw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3brnmkqiz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmicrxx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hgbdndac.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wlidklhy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ylcvhwhq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3dmljjjwo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3pqgmhoan.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zdeycicl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wjvntvlu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3xxoivffh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ngscfqua.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xzeaqmyr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zeqbcljg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ohsarrju.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zxvpiaan.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3neczabie.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfwyjmgd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ihaxgmgx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqbobjem.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcuatkuw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nyanyfrr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgicnyu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3znzgvkbb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tbvvlevh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxrobal.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qajfggdv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gsdrpaof.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uhmentpp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3epavbrgu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3dxwkqwut.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqfwtpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjjctkxc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pbelswkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvdittej.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kqtfqoya.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3cbgdknqf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wmqkqbjj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cfehqdrx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tgjgatgr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3emtzdxem.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdfdddk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jxckotlo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kqknbvet.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kxxwhkju.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3huexnoux.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3twsdmksn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pnqkbpyh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mjzfrxdf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3komhyujm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yotsgfqq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fdrfuymb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3koacvlma.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ryrhzphg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jtxsfsia.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3frxfjpcj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xfhmfnyo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zhnotjim.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tjylkzsn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3siuaihsp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ynngkbip.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jzjcjwkm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vveeodnn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3bnifddhz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecaovyqx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nwrombca.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihxieujw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbullzdy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cbjsiekf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pmffwnfd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cvqcadei.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dsdnbbpu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3flrdeias.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jgtxufpt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bzipkekn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqddtgvn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nfzspyil.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jpxjqjee.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nmyggsco.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3liechrwv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3wghtnvdv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ahrrfuvg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3riwttujn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3noptiozm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3obvbhkru.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3czcachsg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lkgsshii.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jimwjkbl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3btgavwef.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bkapqtim.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wuntdiop.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ehxvzzji.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cedolejw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cpmxdnsh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpzrfjwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mlrucjlx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fmgiyffz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3clfqbvfb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mnutfwau.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dcupxgqb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3objahfpb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3poryfeqm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ayuiqwyr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wsxcaauv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3spzsazja.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qamkxwcd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ugmaleth.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qpefknit.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xfnddcqr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkrdcawt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mozbhyvw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpihqdme.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uutatpaw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3imaqgsri.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nglenwmc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kketbjas.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3olblomcq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gurpzbmp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3drhtblgx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ozejpxke.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ygjzvcmp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuwqpnro.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pyqcqhej.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3fwnqpine.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pflewgtq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eaumbirr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kskxvrhj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gzysqvgp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hgvucgct.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3egcuheow.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3odpcwguz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3aocbawox.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wahegyaj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3szxurnsj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tdfdbtua.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zebhuuee.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jddolxks.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bbtzmhcr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qrdruqax.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rplvwkkt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3javqzmlg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bazgzyel.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3oudkfdvs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fmhkqlvn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ocwnrnnu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wgosjtxn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wruvkzmv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pyuoeqpm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ivrpqhrj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gceqgnyq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ouilzckz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3odiigzxu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fpyncqci.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bdnohqzf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jzuwduzl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xnnnqjet.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvkipgz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xvidobpn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugcicmxo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vetfrwpr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3izdzegsk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kidjssnu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3stojxsci.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zrrkbrla.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nuwnehdz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mbzwjcmt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aevdnhun.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kloiekyl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ulieeqmi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3swkqcfbj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vagydxyw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ajehuozs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kwcvbdzd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kepybzhd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3swrvbbzq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wjiafppj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3potmppet.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zlywmqyi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3enxlnrcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppchtvui.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wkfqaqmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyophhmc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kyqyohhk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zszpafhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gfmxqamg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngsrrjgv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulqiibhd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jufhqoek.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3oazbcfzy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qathltvt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vvvccido.html


<!-- 参考信息 -->