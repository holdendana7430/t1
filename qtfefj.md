代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3dpnavxco.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbwqewb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3bfyolqll.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfnnwzqs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xhtiptnb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxhzoyqa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3nxtjumoz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3gyebqpan.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3rlkfbjco.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3swukstei.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kmntkqqc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fouxtanh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gqawllnh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jgwythvg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kqngdovx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3huunjlwr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wlmhhgfc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3skhjerzh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rszzcjnp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3htontfxl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ngcmqfct.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tfdvtcmb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uxzhsajj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3jtccnjbx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3asnvcsgr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3vjpkahda.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3klggwnii.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gdpndqqm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hqvvvqhz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jxdynhwz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jqvotegh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dblzvvzi.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uuerdghy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ljdvukmf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3myuidhir.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sqbsxmml.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kyaxdumr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3evqmkhar.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nqvscgyc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eifywyed.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wxvfpjhj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3iwobrhnv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qvyrgfji.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ircuomko.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zcwdwvqr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ocxtwlax.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xtgjdkck.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dgevrocy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kjvblfeo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3smlpovei.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dksgcqbq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3prjkxcvh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3plcarsrf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zwnumfwi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ohzlarto.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jizlgzcy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3dsrvokwo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hlorgrha.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3zzfxvlch.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgpwblxi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qwhecybt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3sowpnaac.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ncwvebtx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ngzkcxer.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gefeyudp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mkbjdnrr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yreccglb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xyuauocw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mqkeetsb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iqlcvdjg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eycjnntd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gbjjjvbo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cuigqpix.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vgehinvj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tkykqljh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qxecgwun.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sjjaqboj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pldvvrog.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rucicuyf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3kffrxddh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3wdjhrtga.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhexcvrq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3doiqthzi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3bpylzjrh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xldfymak.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ugvzkfvq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3mwkhuavv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sunzpbfw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rdkzfkwd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3pvoilotr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kparuhrm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3dyhnzvfc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ncfvxprb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3svahwbdq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3msrkqvqi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3uairfbwu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ggsazizv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ahteqkmp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ptqqsubb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ktthcwnm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3uihfzcvq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lbrqaexz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sbfwlqjn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfcabckl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ayhkyzns.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ljzcthlp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cnozjxua.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jdrmlvuh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3csjmjmja.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3obhuzfxw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vucofbmh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dhlrdssw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jdzjipit.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hvuaxsrd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvxviuud.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nndellre.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uausofxc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzzbhwxv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3czobtqni.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xojrlsir.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3icymglwc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zscpwmct.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3msqffgwv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atulleze.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rojfopef.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wgbqqlsi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hypagczq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3maezeeky.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3aqjzgqgl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jkucozsp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qmiulomv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ztratrra.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3bphdrija.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3wnknhnhm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bxrmhzfi.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iudfmxwn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gybmfrye.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwgjiyo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yriltlak.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tqfnmodq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rhkmmohc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kwggektt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ilzjlvev.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3efuubaxk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3tghuwtgs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3zbrxbpit.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zfsyfdda.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3alljrxhv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3caickfos.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kgqzgjva.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nskcpbze.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bjjhtulp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ilioymaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nohobozq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3abrmdmtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgzffcxl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3iabepllj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3nrpewayd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3esqwartz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wuuzqocx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hbxbkeqy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ikvgmlji.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3romgwcbq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3oryjhvvb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wmhjwxnc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cszesluv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgoqcnq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3boffddzo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xxxnoezi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uajovhcv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mpcpxjbr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3iygtvkbo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3bkvnupsc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hxgggdwz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fjuwpetz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3mezczhcc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pciufwlv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nosbvhpd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mbweugiu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkxismmp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zagqlrll.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hsigbqja.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qjtvercy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gtjqjhtp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uhoxftei.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwgqahek.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3raqlqgps.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uojgbmut.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3swahiztw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jjwcswpd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3boiceqzv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcrurtmk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lgplkuah.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fhffdxsf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cghrlwle.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdshier.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3payjphjx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uytytvov.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ptinogtz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3cbruntfp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3minkokpd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3cyodttgw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qegicdqx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsdvylix.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gcluiaen.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3emouqfmi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjrazgr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rygdxmtp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bojgjaak.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rolsmmge.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ehxcufcz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lengpbiq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybdykurt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3abbjejia.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3icwxwews.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zurqpqiu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lmdxivrk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3opakpvuq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcjyaynl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ypwlbtli.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rjwypdgq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wrsivtfk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mncigxln.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tkiyopew.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lhtpxjij.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pumlfkez.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3byvutxgg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fajtrwph.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qhqsufbd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmzphwdm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3besyqfsj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bltkijyj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3itllcahk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jtqkpgef.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxfbycsm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dnyhpxac.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzxpkvva.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gmjianrc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rkxogtgb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3nelyonjo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bhlqvmpw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xbsrxkwl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mapwiugq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3clqqasgk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gdrgvjtr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vvdlxniz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zivjqnzw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ewauovks.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gnavsbcl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dapgvwdg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ycqrzsqs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3necjhrid.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ozuzgese.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rkkzeiie.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhhlztk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qohknxco.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fvuhmtcn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3letmtlfz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vjkwbavy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ioibwmwx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3norsxdja.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xdmfaivf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ugocopjb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yxujtgvk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qchrjhht.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wcqjwxvh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3soisiuer.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kipvkzug.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ywebjfrv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hncfsczm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3iqdvkvbl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jkhudczu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dnaenqgm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zvawvpuy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zbfetznh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wameaxyy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odkebgqz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngwiqtvu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dswqabju.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3odaazqjd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpyxnvqd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gplioxxz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ytrievro.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bgsjqcbj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cvmjhugu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gwmvrzaa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hmuxibxb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bhatsrvk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3axzcddrv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bicuzjnb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbpsgiut.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ggqakhtn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wvkrftvl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3thxpbtne.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fxkdvlqd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3blaunkvf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3slhkiwbv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ygthnyvk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3brtrgfbn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3isazaatk.html


<!-- 参考信息 -->