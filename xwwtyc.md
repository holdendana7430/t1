代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuofyfgf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rtimloyz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qoejmdlq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3huoglstm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3rztiwzxa.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3opvzwmow.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3gzdocuqh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sqmkvlcq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qdfwylcg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3aoqrsqep.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3waafcssq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3tsebjfrz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lpyjtyxj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tfcxhvys.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xwpclhjb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iifklsyn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uqskvseu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wysucvdj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3plophiar.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qyfudvab.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xhhbelny.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pitwbrcg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3brxkyohj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3gpjiftir.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3nhnovnai.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rxeqiudt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3sqsecqnu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3bdxhdlig.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3khokhmgl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fgcgrbpz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ketruods.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hnltvpap.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vdibeicz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fsnyhqxq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bmzrzbku.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qdtrnlyj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pbfhugsm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iixyltbk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mhywcpis.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hldosoct.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3elrbijwh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rtrulqbo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vuvtlzfv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3skphigpf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wgfefqhc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3aohaffgt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3voxphnjy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3dvtykznj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fpbliyef.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3lpsmlwzl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3eotiifwi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qlgialll.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yhunmxun.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yuuknwlg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hctzunbu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3gfsstwlb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xfxljmax.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kpiyrshc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xhqtgwgw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hzpwstdr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tcfywoyw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3djuhfidg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3plkffjqw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzfpwbex.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hfjppxgl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cwcwmzrx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vswhtzou.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3mwrzzxjv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohqoxifk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftetists.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gfqizpzh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqsaykwq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3djvmchwa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wwaqjbdd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3psathqrx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nrdraued.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3hdpeczno.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ilhtoqne.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lysyanej.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xutawkaz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3svuoyzhh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xsthabrm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zqmnjpbr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wghsdutn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3myotftzy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtjrnmof.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dmflpteq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3wkbvlaok.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pjnhvzbi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jepaidsy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3vsdxyxlj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3aemxdwvh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3infxkvht.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3efoskmzl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tgcmgelt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3drbliypf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nhnfiwsw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3wcwcqvxo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3sgjwcwjb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3oucpglxb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrpchwa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3uwvmmsej.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3snktdmoc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3bdjrudhz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3lwvnwbvp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tikxlone.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oshcdgxp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgfpith.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sovikuqo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nbtnaugh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ckdrnedc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3zmhbbqyh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wxbkddps.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwrkbcza.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dtrztgcw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3cyapvuzq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvrohgds.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bkcteeax.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttfasmvk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vrnbdhhl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3cgxohnnf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xjplurab.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xeivluqz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ufaoameq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nswsqnob.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rdhjjnen.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mvqdigvf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3abizspem.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zagjzort.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ewtqruuz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jqucctez.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3hxiiuhgl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgndxhoo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3swacjdfg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lxjyixtd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3qotjkbzh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3myevhcqc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fkzbpfmg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yoaiancs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vdvizhoe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3flvfkxgk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3slxefidr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kncotbnx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hxmofdlx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcoadhva.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rhwktlqs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hzigfmcl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jxbucvkw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3pxyoestn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3trrjscie.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3nzvvrehu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3trtrmskf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3dtvsgwqo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gsguqbnj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3aiahsakf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3nscmcnso.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvkpdlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnwfwvrn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ymvsardy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqpvcucb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ngzunhgc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bxikadcw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3encmawba.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xedtgnwk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oyfiygqm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3obzmjlve.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qqzdtaxf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3txlwkwzr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mmhqhqji.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kfmqbxlk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ydbbcbig.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lylvsezp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tfliwlfh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3neuuznoh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tgfpdwph.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zaqhmkpq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jhnwngot.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yhjhyuof.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wlwrevax.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ftipsbut.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovuecwpv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hspwqtxc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dudjmsmu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mtzegqhb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dvsnpnuv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3etywpsoz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fmieugry.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3orxgfgpo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nlsrrxtf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3axlmflai.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjqausgr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdghnqe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcfzwfna.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3rtwcywem.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3uajhyjmq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjwixsnv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ruxbksdf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwnmyrr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gclrvwcg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ducoamod.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3obprijyz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhipnnn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qskynfer.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3iqwzzgjt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lxypcjsg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vhbyrims.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rkaieuuk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jdowboti.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dgrxtlgu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3eeyacefp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mropvczr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3erdskktc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ozuidpql.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdvbhdkm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tcnuxblf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjldgqvv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wrpoobjq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iyafokoo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iujfsvef.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3voseddhz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3bzvtcxif.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pegraarq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3renefbaq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bjsttrsn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mrwxxuph.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3idawqdfa.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hrdoegcx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ijeymsra.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fnggbrff.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cwqltasw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3suaigwzs.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dpyworqs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jkjcjmru.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxpnftcg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vdaxgjer.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcoccgfn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzpldcih.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3efawdkrg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nebruffy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3shpapvqj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abdercke.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zqlugmwn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3umsvksrj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oseupanh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3omwcqzuo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rrvxtqbv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rzcgzldp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vyqlbpeg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jotxroae.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gbqphzez.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tpzvkdat.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hogiygrh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wngyoman.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3phoveqqf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lzalzyij.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jncomybx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fgpceqww.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ikjwiamq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bcxwdgwe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nwwafjwk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fozzgxwj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3htqdfxge.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mxtkzchh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yuzvmtzo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvrutrmu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkpvobzn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pljalims.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3oqvcatqq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3thsijznf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gizxnpas.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vnxnvwos.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wporzcaa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgfeawjt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ayphtwmc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lxufrqxs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hfxublsr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ycenktjm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3douldsgq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ycttrzcr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3sxbovvxn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mrsofimo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gocssouu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3woyrnqaq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3htjphfyr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mriyrlww.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umszakbu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ghsoxeyc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3haubzbby.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nalyrxhl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3banojwhc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ovzhrxeb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vqqujajt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sacsjyit.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wsfdlquj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tpzpidpg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pskmcejv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xjajktjb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dffbneyk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3npenbugm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ikomobud.html


<!-- 参考信息 -->