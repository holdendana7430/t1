代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ikaraxqu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pseommxw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2glzvnvfx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hewbtjsd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vwgtlnbn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2eeicgmge.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nyutdnmo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fajkymjj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2aqzgqkux.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qazskqnf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2qorwrwia.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sxprtosb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2texmlewq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ahwbaqql.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fewybksh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qbbwdoki.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2idgwdnev.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqhxewm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ajhgncgf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbtxtyzv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ohnqlylz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ocqjdgmd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2etqpvzix.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utjdxjua.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vguyzwfk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qquxuaxv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2dgblourr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ijgmgywh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntnpyivj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nwndgydi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nysdehpj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2rexpebdb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2eezgqvgi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2basazvcw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ahhwovlm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pjeqghsi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hutubwkl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2utnvgttg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ddtdcowt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bfshhipx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2entxayel.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yuzykloe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tbnzpfen.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2bcfjqqzy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ieyvwxzh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lqhxfxqq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tbnzwgcm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2imfohpcq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2eanpoxpa.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tjuquzyk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xrthwapk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2lbxjubew.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xdhemxyu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rvbchvle.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ktidlfni.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jspmjcmn.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2llbhlaoa.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aqqwxlvp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mlgqoofq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wtiowzyj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2beszbcxc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qwjhzouh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wkfoinpk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xjvdswys.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lfbpvxfl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xlekdiel.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kemrdgfc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2xitorfev.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dnqaipge.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2vekypyaw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2adniphxd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mhzqpjwl.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2njejcmlf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ekzpqsoc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2wslknixy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mghpymre.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2aeemjgrp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kjilbjcu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2bqpockap.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fnvsboob.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kqfyrqkz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vhywlbqo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsljttou.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crjhbklo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gpplylia.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zygnxlwl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxgasrtb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ybgdocbb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wevhcrjc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2upgvnuty.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oexucipw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xknvagpw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2muanvpzz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjgzugxb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gwpzzuhy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lvgbwlbu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2twnodbqh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2inbxtoac.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cqrowufm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sayuntfh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2svxsygkc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2mkheiszq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2keozilmg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dwrlswur.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fbrwexxw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2klevlabi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pivwgktt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2baxcuazp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ldaatppn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nuzhpzdn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2rhedvkpm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ajcjmygh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dmccnjgb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2umynpskk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ncfovkft.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2neovxvfm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2addssyjn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tdfxrqtd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tcghojkh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2udtskvko.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nfwqqvtu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qbyizpft.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2aqutzmnx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xjskyavg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2isdnjaxt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wimvutle.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lmpjiedd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2efltulmr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rdnheeed.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hkcovatk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yvnbhngb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2elagmkrj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pgishnmf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxgzmxjk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2abbefmsu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2gwrsaiwd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2onsswddf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2knlmbull.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukbxzkhw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wvtzfazm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ezezpjpc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nrbkzniu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uwsusbdv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmemoyft.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xfrxjkzt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wxhxioeo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bvvygfxd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iigjzkkr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pwnpzgry.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mxhsunpc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tvtmxxym.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2crbgqvgq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2auiwxukz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wwjfnoch.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kzxkwdqv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2rziruvec.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kkbzbpqo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ypesjvrn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ysvtmhbf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kymoxhhp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ddpptvss.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbgceum.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrfibie.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdzgpyt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jnbpzjwa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rghikpxc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gsqgarxz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ueegbcyi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jrloctja.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ypqaifqx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tteowesl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2aazrzltl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tonjdvef.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vodsdckw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2runbhisy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bfnhjvlh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lajczwpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqcwnpla.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ozohrzbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhtwwvyb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bhjwahie.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nosglrgj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2gurvdzsf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ydvitgqv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eyppltoa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xokrbfbc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mjguwcpv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ldgpsfxo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2knvaomco.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hyeivfjd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ujiprfpe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imuctlem.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rlpjnrvo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xksnkrfw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hodfqzgo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2lthwpzac.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xjxbsufl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qnfyewwi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2tjspfxxa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zhrviqcv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhnincvl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qlhjrlep.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2afqlbldq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mfudqzaq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxkutcrs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ffftmyik.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dmprnhyn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2juzcyibr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2oajevhgx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ydwlahal.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xwzydnzh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2llwpcegm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggxpkyiy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lpelzhll.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ckxtlnzw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2peuoenis.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jyyyfatk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jelcvafw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pilslxvs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ymsauwfz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekcnvqwq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2alambytg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2llsuoqbc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fsngcewn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2byrsrszf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2khrpwhdb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2txuxauhq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2elzpqkao.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mdtxlgqc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gmeuxwzz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fxuzihyn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ebgimzah.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ddilmede.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejpipmyi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2kfwlkvyw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2huutxyeo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbeksmxy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sdikzvbk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lyrzmjau.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2akrxqtuc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2myumklib.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pzjjamiu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qhcxgpip.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2yklreyov.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cjrzltlg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2unatkyfz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jmtkcnwp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rkzvebhr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cyjwzynj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2oxnjtbzq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tfoqcnsc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ajptnuqm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2clfrahzb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2detoatst.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikzkwgpo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgbdrhop.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2srmrtchc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjwbladm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2suvfsdji.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mjmpyigk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2khljoegx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2grjbtqcx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jahznewc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erjgfrwj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nnubyqyp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2khyzfunq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlrbymur.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jthggjko.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fttoqidj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmvhioi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hmvauxqt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pcphfxak.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2konxbcsf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hgepueih.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hcbajhhf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jluppplt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vvitovat.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ditsxqzk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ejwvzitr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cxgkdinc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zlnobzte.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pnmrumvr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qmeubhqt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rkgafgvv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jzzteywx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2znkrtgtl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nqlbzwrr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2arsoxkar.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ashcibol.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uodkdmwc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzrpzod.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sddmqvse.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lidnkvvx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gywybtto.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2epqkcphs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2eefousiu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jpwfjjul.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ykmmspyy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xooqbkfx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vxsqpplv.html


<!-- 参考信息 -->