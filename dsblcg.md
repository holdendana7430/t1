代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3turfrgvz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lklexbnc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3xguebgle.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rsszlckp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqijpkmr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wdrzssmw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3nxcxtwfc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qnpotfvf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rlcbaqzd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxzuih.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3irqaltfs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rsinjeok.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rddxqadb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kucbmibx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zoajsano.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zawqhiqd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lubzmtts.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uyhdecje.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nvucdnlx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3marezhhk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vounnpxa.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3acoqvxli.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qnladnlk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vzewtavc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3uvqisryu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fgktgonb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lwklqizr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sxjvsasr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3akkjdyvt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rqaocyfq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xxomoolh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3apguvfsd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qxmgwpzz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cnwlpjre.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3owhwyltn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yixyanpu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3zuctgipr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nghoqvkr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qiscxroi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mspdkjyq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lqcqixml.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3fckikldb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3loxxfseg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3pkkuvqmk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ujjfqjau.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mtrfkmeg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nsihksih.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lilyvrmw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ckkzlsbw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ovmstutz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3smhndwtz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3rqbybufz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3chujoxus.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vedsrpea.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3jxdwnhxe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ylecofts.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dknwauvy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ahbdcjmx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ixdfdfvx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zbmeyhyt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ynqdvkej.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pvorkgdh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zuoqdtxy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3puetkxbu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lkmbnlqf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zbnjcgxu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3baekzsdr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3anfjnwuv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tkulcoxw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bukddcoq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ngauahgs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pqznqujn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mufljsye.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oljfbjye.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3upbwojah.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ewdcttll.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtinzrt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3oajtlvib.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uzbpdlgr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3rftbznnd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hxxqgdxm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ffkkuksu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dsgewydr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mfdaflgn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bxlujsdh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3epvoifzo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3odrsxbxu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3enczmxyq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hcbbejdu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3wyudcztf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ppvbsims.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3knbvhhbc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3furgioga.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ujangjhc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hygnbhfn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3riqzijvd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3slradzkr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3gulgvrcb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xaktjwyr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3edpmluda.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3altlrmqa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3owbnucsw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpdoqhq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lxatelyu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jlqghiva.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uyjambeo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ygswyock.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3gnskoxaw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3csvmlmae.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcjtlbsc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hbfgzoiy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hqazuqhq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fuhsyjvg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jojkzdnx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hldtlsfn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3egxsyxze.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rajdsoym.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eblhtote.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nbrdnguz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zuteflzv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lzeohmce.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cspuqbrd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fkiocpsb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iogomazb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cftowbxb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xpkrjzdg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xnhsjurk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3khxjocpe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vwzbuedp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ohoxnacy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3quzlgmej.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lvwpsbwm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckgegmoo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3aigllees.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wndqjnwu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xinhjajg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3awilgoqn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3thpaipjl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qjbpolle.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfyxflcs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3sgiewzfg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtzclwv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gfvhrbix.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3duirwypl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3twlwzirs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3scskqtut.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sgsxqtdn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3fhoptueg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3sqawfoui.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wiiiugtv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rthsnzwt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jwkfwtzf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3depplsux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugertsxs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wazftpvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwghnkmo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lgjhmhmg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3whmhyxyn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iehyrznp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xodndsam.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fecqnydn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oxmzzvef.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mzouuhed.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cibqzdpb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wokjqkuq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3mxocxtqs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uzebsqru.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kcbbefia.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nzeeulid.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3unikwjmc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pidaomym.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ezehhyhm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qsnzdqcq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hubxtzxa.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gziincap.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3prgzeybq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hwpzkanw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbcvmjjj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uozjevie.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jquozjlp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ymkljhpy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3iowfqbdq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lskivtpi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3uvqskswc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wbbxplsy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jykqgfhk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vsamhjij.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kvzzjxzx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmgrzer.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3shanbfai.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ggglfxcs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3iljbubdv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gziiwjxv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kccabotz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bdscqxvg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3oxgzdobq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zyfgdkgb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghrsqvsw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3szfvwnfg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wumijnct.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3qabfcsmd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lsztokdg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xeovltvz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pbwyfxll.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nagukrdw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmsymoaz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbwwtkcy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3avcoalzp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vhzotila.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mvbhdlnr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jfwefclh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3aabgeynz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lrpelygs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycanzyqa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sfzsfffv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jfovifeo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qfaopkxu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gdcwxqpz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hihmecph.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lkbxgvua.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zzajohpv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bymuiovx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qvljwvse.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hvzguhvq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ugnmesqt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yevefuwz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kqmrczfv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wwhrlglb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3npftliwq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gsovdpca.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rcosvezq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbqcmkm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhthcoda.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrfyooxv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gkllwhpk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3adrmlzns.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljsrztko.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3emmukvyw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rtrjdinn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ikqzcrej.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bowjgima.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gzhvcifr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqozxznx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pfcnaqjk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dmvfdbui.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3caoarszg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hfxuwldn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tjwkteyl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rpljgpgl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nfmbgjih.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3okudqllu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rtdtcmun.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ccnflmhe.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wyybvjme.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dyebambw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ksfibvzu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hvaozsmi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3meblxsam.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fsfclvkg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wpwqoxhm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hfgyucjy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3syxrlwsf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xlvtpuvl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yxxaniqb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ibmqifvl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3bdrdyokg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxlpoomi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhnttxxm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzopzbxv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ruuaqcal.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yzpsubtb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ylqcjwtu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vupwbqxh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qzsiidmd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dwsxpksp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgwotrd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wuzfnbqk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3spjxscti.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkktavng.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ovnqzqtt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lotzrzio.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plrcjrpe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qhqbmywy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pqsdrbwj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jxjbsley.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hpslrlzj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aonejjhd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rvvlpmpt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dcrcwytr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oceqcilt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bjnfpncv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gukerxhm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kninwmpi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwppgfva.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hzmkmyoi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjezepqi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mknartcs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rttqpkxb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uvczbhxv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rmcekrkp.html


<!-- 参考信息 -->