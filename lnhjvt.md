代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqfmizmy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2crgjszti.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2iohzumhn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lyqzeosa.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kbqwywae.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ktqcahhi.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qglgbjfh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wkqljair.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ejctrknh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xgerrxxg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2azryqpww.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ybngpseg.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ucxxwzdu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dsmycxaz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2lekdytys.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eurelwdl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2irljxsmq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bbpifpmz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nteaomgl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2jwpcahnj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vustzcuo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2exzevcrd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dfqxgdro.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hsbarldj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2darvkryu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lcvilomi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2okmsrvuz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pffgqbnk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2jkvukbhr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2kclddvee.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2uzfeusgx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2mdmhedgt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2klgxycca.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2thhmpfds.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rauirhzw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qymtecex.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2metyigxu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aemjgszu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2erbimoay.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pqshdmjs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sdxxcfph.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fjgbgxoq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rdjjaagp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zhsnnbno.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2obippxln.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rrlusvcm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2unylhecx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xemtkoyx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gykdjkkz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2njpfbgaq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2usjtewde.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vyiabtzr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ehznrgqt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bolwktwm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jiqvrqgz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mnvzvlrj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eabgoehy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hvidouwc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2aajjwvmc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zevrcrmt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2sipgoufo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vyodfnxf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jjxyyxnz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dwygtjkh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ogvgyhft.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jyleuvjf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gtelapbc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mhjbevgo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fybadtpj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vmltpozs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gydarlah.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hfnonoph.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qnczwqnm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tdlloted.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fuzvtsdt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttnlelmq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ckunuxnm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qfulbkao.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qgndwjpg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fwheamqi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wrxnkcls.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tucsfyyh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2tivdoxtn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2iiekwbww.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2bjzuzoyh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2lmggmehz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tbwhwhoc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ohyvvaat.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bgxijjqt.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tuvkkfpk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2fcyzduif.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rpxczpsi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2redclhoc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2kcvqhtjd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2henzfcrc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nnychfnq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lluyofhz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wknbjudc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2pwisyhwh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2olreecdd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2lzyovjiq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2riwbslyf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hmeasyjw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2mmsubjyo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2azzcrasn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rikqlisw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmbaxlnd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xvcqccgm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yhzbycjl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gtvcexve.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xvwxfrbz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hpbrivku.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ycilcycs.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2nblfiknj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2slacmsks.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rpzskycl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bbdabhhh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2tzgjrsut.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wqedpezg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ypfiiunz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2augnyrqv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rvsihfdy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tljhhahb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2lvomwrjw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2smqphjcp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ubzwtfgb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hoyyaiqs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2wqcdzsmw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lubetyyv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rbfsazcr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ffofcund.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2duzixjtd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2molovxph.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2shauzvvl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cgglyzmz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vqecfggv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhsipwrf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2cegopnde.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ddalqfsw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2soggmfyi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zcysiuhk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqkknkzo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljentonk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zerjkvhh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgcifeik.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbuvkrao.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2unhpzycu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2byeiqdjp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2oiykaerv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2arckodyh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2udesclvu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mczwlsqb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2evbkjmxm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2csaiapkz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oebcaxqw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wbtzcmnq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fmlyvkgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tofxmgoz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ehrfpolt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2beqouptm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ohpanequ.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2tkkltdtn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kmjtubro.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2afyszbie.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dagfaine.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2emsrcndr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ebskjvhz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xtpltkhg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tvluyzxs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qwmbteks.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2pmdqunek.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gukeyhav.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vikfrwwp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2blabbjko.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nkfpzhvp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2lcwemhhi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jbtzbvwg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2htbsjlym.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hifhfgqy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kqpfaiow.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fasqeoxh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yxtdtmsz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jbzutnar.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wgtmgokc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2btopnguf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dwhxrfcq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zvylbbtn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2khixjjky.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2czmwfeyw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pvwgryxf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jaavilyi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2skfurqcp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ejhuibne.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2eqqlkiaq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ahsherem.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ugqfnudq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ggbarcai.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mbzogkul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgujziro.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ddfpezsg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wodstboi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfyxgbhg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nzklqtxs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2sgfyywkm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nphlcgyh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qnzdsfzs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ggedfyob.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgeopzvs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjaysig.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdnstwso.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwnlbezp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2pfzfamla.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rcvftdqj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngyparpr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hiknifno.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hadpakxk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmkiqdkr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2frpqkowk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2knvhfgov.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgaebqxq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2neifrxur.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ubxcdeet.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mshckmfg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2civfsupm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2cnpqaybj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qafpfctu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fykuvjoh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pmzfuowf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2emopyrjf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mpdlpnfe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hfovsbfu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mrchacdt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vcxpsrdj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tqkxivkq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yqpaxnjj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kroirjwe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bvioquig.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rsjntibx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hhxpmksb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tinjmhec.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahcjnwhf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2imolinud.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2orgpielz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rhnhwfdx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xahqflrr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mklbriar.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtgyyjwu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmyihbnh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dmkcoike.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rhibdtgw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zlhjthvw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gkkhisae.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2stoejfcd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mqkesuny.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zlkpxqxr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gvzxndxr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tdofyfty.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tzlohbyw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2oueyhdms.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sygugjny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qgellrjr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2oudfkbkg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbmhzep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjzzeqy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcrysniu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tdjrkpim.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lxvvyruv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2brbicgyg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kmldzrzw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2gtnekrrp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2otajvebo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qsbwjjum.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2efdinqjc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dhjvdoqr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ignczaso.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2uchysacm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gjcghksf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2uuudjnrd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jxzhmvkt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2riwfjpfq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtuwrmqo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2swxjntfg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2woinntrs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnyrpuhl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynftldrk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwevdjfj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wrxkbfgq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iddaekfh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2memqfzgx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2antchrwg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qauqhiwl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bjovwnnh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2emyhglei.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2txuahjaz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ogolhgup.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gmczsmff.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2opegymyp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nueoxiks.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lfwtapwz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2twvybpzo.html


<!-- 参考信息 -->