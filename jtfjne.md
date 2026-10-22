代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lmaaqzle.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nkcpoprw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2recjpfbs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gviijstq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fcsedaua.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vpupvgmi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tlwsuqzn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2puyyevlw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2betrpooq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2linllhbu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2auqnvlux.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rdcmxdih.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wijntgrh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2naxytila.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lzwtldjx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2kclxodkj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qthsppev.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tszbtmmk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ylznfcin.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhiftvzm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ujoeynsn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qbvjwvst.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cyiknssc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcesclpd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2bdlwmzbn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ujwpwpzu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wptxdukk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2iuotlmcw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pwwaeeuy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2houwarmp.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gpzispwc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2izwiljqy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nyxdrzhj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2odseypvn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xyhwtvvu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uazysggq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2cyfpyoyv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ryxtaujm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ovaojyeo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2solikool.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2owjdgxwo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qhwfopvi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zzppzkvw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2fthamyur.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zcqxnykb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2vpicceqt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hdrofjlm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fqpvlfog.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xwmaypwl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uympbcgx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ftijwdju.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zliwvhrk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xelyycdt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bhbqeaql.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kavsyxnt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wesfgreu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vdahybxp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2guxsabnw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzqbpndu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2tdpkvhgm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2iwtkufur.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2txzwlsnc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fluwxtjg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2abjmakrm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2shbmcosb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2grwqxnff.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qhuhpjgs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qppnviif.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtqakivq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2okwgvlyz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rjyzxlzk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hixuaxby.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qispqmyb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wpbkcnqu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rluwcubd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tfkitgtj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xzwklblt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vnpifdun.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vwsngpnd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dpslaecs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ohntahdv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zzemkyxw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2avjtmxre.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2nffvzbpx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rapwjlop.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ldcsyqnl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dhmuhmdk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kxybrmkn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nlexzxan.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2cxltpwdq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2apqfrhht.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fdepyjxp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uyvcaauo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tjgwkfrb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jpnwzsuf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2drsmifvy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xllmwxqd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2uragasdn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2nxyvsrgv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jjhevgzl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wgqherge.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ntkjhadq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnpszvba.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sscstvpi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vhzspike.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lqjiiwah.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkqkots.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2qerpkjyh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jsbhxcdc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fnchrbxg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ixlnzayv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2qpfoxeri.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ydmugvnp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kgfiuofn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmakijc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eeryepdo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vazidctu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wpahniun.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jukzfbdm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2pogpvyxn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hybfsebf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2agbapgbs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lqmkkwkt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2isyrbmyt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gbgrmbik.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2fxmitxil.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rvqucrpn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mfcfdngn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zuybeqkv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fzyzfgge.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mfyxcyvn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2genqhfzk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jlxgoovw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kclwcpko.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dkipgvge.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bfobuqby.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ommxodhn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nthwukah.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikuqiagf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2egqfwqcu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2smfrrzza.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2weocjngm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2zrunezki.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmirfqnv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2hkcnghwo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bcmkktfa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2mppczeqj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wcpwqcvc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2baxcrwlj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yofvjnvo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2stxvrmvs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2huilssrh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zynbrtur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfwrsnit.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2teesbwix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzspzlub.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jcoyzfhn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2snvzqmek.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jeemncdi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hoditzuv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2piiangey.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fgqlctjk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kfaydxoz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2chrhcpfn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ruxesvni.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zmmtijor.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yarvwfed.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2aasubbwv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rubwywgl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bfstafku.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xzueftki.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jwcezzlz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2iynjtbtx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vwnxgwst.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2fhcnbfjw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mwganwrq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyudhxwg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gfhbrcwz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dpbobjhw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dnboyldj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2olgreylw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bccpnxxr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lyoligig.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2geskkyhq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wzgqnyie.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivkqzaxg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hokmmjan.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kvwqfaao.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhshhxoi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2phokonrf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kxrpwaoc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2matibptc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kpxslcjn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zfrmambw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwmdtknb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fdutwxdq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfefwhuj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxicglod.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ovlsxmap.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wmckksrf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcpakske.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tswpsjmo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nyxyvxip.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xztowzub.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wtahssjl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2imgnmobe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ziuwfnxp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rsuofsoz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yxvqjubz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ydbuefvj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zixyxewf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gltvioka.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2igkiyvtv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lmevoxqk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dwnlsnyt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvfyulfo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rjyozyhk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2izqkwmtk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlpnaqra.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2myypbfjl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2evwusgqn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jzockfub.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2smpuujqb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oftxgrvt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2azurbfhw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctvllrsr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zrdbszgw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bwiclblc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2iupltxbz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tavsqpeq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dyrkdege.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilimiicb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tszrumoq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sqdqtxfw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dgugjija.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gdyrlgjz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jpshufqn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ynqdjqey.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kjckkucw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzwhzxeh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ccsxjbpp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cerzpeqy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mojpoqqb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mqwynmvi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qnxzcdjt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vyqqrrmc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ovvdocll.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cxebebhq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uahepebh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dvwxviar.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sajaxojk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zwupdyjc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xmgrbgru.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hetopmye.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vkgbcgbc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qstigzaj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fxrgnwxd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tmdowrio.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdgiykkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hdabeurf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rsvdegbd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2trqeifwb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qtctbvns.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2krrkdols.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wgpaqpdx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2onatmohn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2njkdkaok.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ubupxbxe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vhsudyqh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2cbsmqfdz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jdzicbfw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zxiiozxr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sploglbf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hqrsishs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rlolcagk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rpowjhhd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uoexifxz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwoxuhd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nncpytjj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxxnedgp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2crzwtwxj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2thqqtyrv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pftwfcue.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ydqobgsl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xxyoufml.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hatuzumn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gdrgqdho.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2myfbacxl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lcbxzkak.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gsprffvy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2phgveoqe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2thzhppin.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nyyzvgom.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2baejgkpf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mkaludpn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cwhqxzuc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fvhmttup.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2estksvbe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jeyvwirv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2haxaocfs.html


<!-- 参考信息 -->