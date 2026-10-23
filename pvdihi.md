代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ontxpwhb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3fdfmsmpk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3nacpuzfk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xwlqtqnb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zudtxels.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3esmdkwlv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3subrnjzo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lsgzhtxt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3eaxlahdg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ovcpygnt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yggoysbe.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mplchdup.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jwgkhtwo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3pueimaez.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3clvsxygl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qfwnulms.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rtebsrwj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rfpzcbrk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lxwcwfsu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3louiiawj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tedblthl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kainyfvl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wwrqtobn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3qwewzzch.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3pyunzafa.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zusdcdqz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3djopjcef.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xczdbksx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3nbryaeqp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3noejnwle.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3qqzdnzza.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dpbzmckn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ukgdgiru.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kyczrfpf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ippplddc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zvvundix.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ofcgfjlo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rufdqbxt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fvtipptm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jqfufyho.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3foofxurp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zoaoeaaq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ivvbvtne.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hlflfvgq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kkvplwsp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pepcofcq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ergpyrhl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3sviwyaam.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rnmrjcty.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3inprhkis.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ofctwazo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fesvhqsr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ieojfyym.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wkrufszv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qukrumgl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3lrtxiapg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yywfvagp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zrovkkwh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3wieregch.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yihbvwqi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3nriqfcet.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zwbxsjuq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qctgqwis.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3syojgowf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3evvjlzoj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3afvgmkin.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ipzqvxcm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nkugnkvv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kcqsimnp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3itjlepne.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qlvdvtie.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tjguoyop.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dnssunfg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dpvbixkb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ihgmxqgv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xgeyoosd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gzgaowvd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bnduykya.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3duyxnbbb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mbhsqhdc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eoyiifzz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3oofwbuaa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3pxqsfcqc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qawuamjn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3apeljekh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tnjizfly.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gffgwuqk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qqakrcqc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nufwhfge.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wgxiivny.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3uhrfbuph.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ixhqmvcw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rthouwtz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3rprbghsb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zzbnzbzd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3txhsdtlo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mcsnjglv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fkxfhkjs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tvzlzpwe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zqbhgrtr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3cognxiqk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3iueiirzm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kagfkptd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3hcawdqhb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3xbookity.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eebbfpkl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzrnorcj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3msrmgiyh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yqjxrhld.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dqrzczod.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3crsgeugd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xeffoahw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jkrfrylx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmhrcech.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dwuwferw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ewfgccrn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dfhejyul.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ozphozjf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3eoarmfmr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pvwqnayc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3agdfrldn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qvjnshwc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3blaomwgq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3dwqicbsv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pexsgfvx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3apcosuao.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ntfvfyvn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtigonph.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3irgzqmao.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tyhmwrus.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pcyqanol.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ktfxzrpp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lvoeivzl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ckbmrcsl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rhykbrhf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ugzdsbcv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsrqyano.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lueevnlp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qnqvzmuh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sqxpencv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3eulcmuyl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmttvudn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iewtqxls.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ofreyrnf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3caoamgbo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3traiqmrk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3dpommfsw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yocwbpud.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3dadadqtz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gghhnrgy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ciwzleei.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vnfjanty.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pnaqpext.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ikcrrdho.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tuhbauip.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tobxoypq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hleiviaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjhtqkxn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tpdivhje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ankfwtba.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3htfdauit.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qqvdnhuu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpvgkast.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cvppdeuc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3endapvwy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ghfxdzri.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vgpkxclt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lcwodpyt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xwioqjzq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hubblxsd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dfiowcfq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziimqvev.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qxyoaigd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gnhdloui.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3romlwyfm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jcwpipfb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wdrapdpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jfihlsde.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3njvnevnc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dlhvazpb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlybpbrr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kgrcjgtr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3asfbygvo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eojpswae.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhivhlp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ajonistl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3unluripf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wbwwcfnl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrheuiu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvstkkf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vctqeijs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3neswpxgb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3frnzvoin.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fpvjhdzo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lmfqvdsg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymsecpyo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3whftqfln.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kmnfrfur.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzoabvfq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktexvbae.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zyqushyc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwhzbbvq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pheuspgq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ofekfrvk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpppvihj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ftvwvdat.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vnmuhcoq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ocmvbqbw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ughteubc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3akpgkfrn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3spigncss.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3duuxihyq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3piaulxqd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wkzatkeq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xpnlyysz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wrpomyzr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgdvsddy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eetnpmws.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zdpgtlxv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3siqdralh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rtwcaosg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3agfhfgyx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kphjbwbs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yadzxklu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hghlxqwp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wtknezhh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3coevbjaz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oizmeorv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xqxxinyk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hpyckrzh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3smpxenez.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nyoqdmcg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lywkeogz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3owbnqujf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ptiylmvx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3phogiipg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuyppiyn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmqgkqfe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mwnexhhb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bnhsirle.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnupuvgt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cqpyhlap.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cjecdmdr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mqnglqqj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3defxzlrq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3woamyeph.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cpnggzeo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tvphduqa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zliecdqh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjroksne.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xrnxcsxq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mkeiovch.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3igsedzrz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjuigehy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ozgtlisv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qnblvlod.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nidhngew.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wsozoaul.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yypoibrp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ylshxosl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wlmgsyju.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gxyyomee.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vuiucwwe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sdkqoijc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vuubivyi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vntuwijp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3lbrgxxni.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3odouicmo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vkvdqtyd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3igaguukd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fumtfmou.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ssmfuprj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jecwifqe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gmgdszqm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dnvrxrhj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hdcrpwqj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lmgeiuzc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vrgwolkw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hfofohgc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wdwxyxgt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvutxba.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uaftjmfk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcdtalde.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbhzeisr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xccsobkr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umkeorln.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yziarxhw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hnjmodko.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hbunvtnh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wduopaek.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jgwgfodn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sxjockdp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3znfyziah.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bsmmzvsf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3josivbzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vvidbzrh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ffwrbbtf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vikkruxz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wgrdopya.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tgadhlla.html


<!-- 参考信息 -->