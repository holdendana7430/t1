代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lsauhnsq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3byljwgcp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hcfwcgdh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zeoqrewr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zqmnwhic.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3andvtdai.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3axtpmxzg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pggedvtv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rwyclfrl.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3esmlgdxy.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3gjdbacqo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jknxwfcr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3nsscdnwa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mjlpvsea.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3euxvsdfs.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rshvtmep.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3mznlbkss.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bhwfboud.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3yxgmqfzm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rzpuxxww.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3znyouzld.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jaysjivp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3edmwbftx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eknahrwl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lifjrmyv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3tpsjtqbh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3thuztfsn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xoaezpqa.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucjkddxp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lebdelhx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cdpxdkwl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pmjwskca.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kixrrpub.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wmpjfmty.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3hiizbofn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvtemqz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ntzpsgff.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fpazhsgy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ctjzlfsr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3solyzaiv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ffqbdyog.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3htsziahu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3nymdjqqe.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mqblsafy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3gflorozi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3yzenhhqp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cvaatjdu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xctyqbvd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cazhfuae.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gcuocbng.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xgucncfb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3yajnsqyz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jmxbookh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bascmtae.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3xifcnjnk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ivaqrauv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qhkummrd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dubwtqga.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xfhpjlmn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3sogxaznz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dcaypipb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nxgadktu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xgjzgvuk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jtqjulib.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zdwabhde.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ijbljvwf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cerihptp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qnfadcgx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sqztaljl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ejvfnqgw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3orakbjip.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rnplcrgo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3covltukj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3enmlzoja.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ipghrzvv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3axclqdgr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3inmjaqbp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xtizhlgt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fezwpsoc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3cgufmmsg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nxxoljns.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3svrgtvtq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zbnwewac.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rjbspbwh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hzjipvxv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oxvdrhvc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3efjpwezo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3botbvmdu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qmrzbmqi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nnjnebxt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3shilcjqo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3knonfguo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3fgcelrso.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3oeeipjnu.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zttkdosa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uflexmis.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3adlxtpbx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jbhkmips.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ldplretu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3iltnrhwo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3knjhhitu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxgxhfht.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pphogdyh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xoxfsvvq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gflpzoqv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jewizgkb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3npwkckwp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qstcoqce.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3byhyahwp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fkslghsw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjclber.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzrvbzw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tefxxwbl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ytskgchk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3aqxcdnck.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3vhtxtpia.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3pkpfjmrc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvbukepo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hjcwwsxj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3chievvrc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xfyowwbi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3egklzfwp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3gydckkdr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sopmlrji.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3udxtzcmp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nqxptjcz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lnqosuqy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3msmswhlz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3fgboppbh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xrryzxmt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3awocdqxf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vidvdioe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3fkixlsyp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3yfxjzkxu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rfkpneli.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xhlkwycj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3zupbbgve.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ewwnpgvq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xsyflfyp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmjvnvr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bfhajivl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zupazvkz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qnsvwxqf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3simemqwk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dfyrdzqv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3bkhyedqs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rnccaypb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wspehktt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3oxdkqsjb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3csfrrejo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3umfsbwlr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3pjjdkfvg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3oyddmwlh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mtvqgxpo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3otwbwrpt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3apbizuzv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nkgbsrmd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vqsiogcp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ldjqrcwv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snrioikq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vllpsfra.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lwpdedxz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3phsfcgtc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3laxoehbr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lmmiqqtl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zkfbfdyw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xossmohg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3sitllbuy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ztgvrmzc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3uxuxaxqk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3exanrzyq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zklqzxmn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3afeqolxg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kajxpbyk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sdpvzapf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rtrjknpv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3alnkxkdz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpygqeif.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vjbcvfwz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mawhyuss.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rffxvkye.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3txodtfmx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qenwejtc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gnrdkdjs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3sunbfsct.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3alsedoww.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3otqlwbkz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hhntgojz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qhxznyts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swhfvmfb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zqiazcxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhsuuqha.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kvgbeyrx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3itawbhca.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhxzicfa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mosvtpjb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mukftfnw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rkznmcwu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3isilpshc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3evfctwle.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dwwskxlb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kcwialrw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pvenrrer.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpnhqlka.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xbbqrdnd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pgyxilbd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pwxrfxzj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yusrjhde.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uotxzatc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lmzlvhhm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ugadzwcb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vhpulutt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgqyosws.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hrjclwvy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovmsmjfb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aencnjca.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ewbafigu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dsbqdest.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ajfiluxe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sceqzadv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fleitxhm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3flssbciw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ontqioro.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3llnssors.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3epkmhbok.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kcnihkcp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xhnrjirv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3jyfbnitw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3khkuvlus.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uiuooftz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cvlnhceq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqadjokn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ixwicbbh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlobdrzs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ozfzemvm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uxturnez.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jkmjiiwa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lbtokmaq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xiaurfcl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3csghmhhg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dytqhfmt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dflowvks.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3snnbviaf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rluptink.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dzpxwvsa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rpizyoam.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kmykqhba.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwsxrsyp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3shzsagtc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdqgboep.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yddrcusa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzozzaki.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3sxuymxsj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gtbkmdbt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qiaxkedn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vefojsyv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hjznjwuk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3esukdovy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nvsucioi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gytfrysj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vrlbhnqj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mbgitsyy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tvfvgioa.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jrnzockq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wkzrfnwd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hgoaymyk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mxeebfgc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gbytobwu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gplvclye.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gwfrxssp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aumzdamt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tlynmqwt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqgmkyty.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qjjrdwha.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wpefzyra.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmvxvnxm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3udbywyrx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qmfpfrxu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nzrpnycv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3llpbblsw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vkpxphcm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3sepwgesl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tdeecdwr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lzcrvolt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dphpqliz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ezczpnng.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nteigkaa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qjmnrtgy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gydoduwg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3whjmhamh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xfcqmovh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wuqqjjre.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3eehfgnli.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gsuhpiqy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fxnxbpzh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wjnnugbm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3utigqmym.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3jndkmnmd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3opbazndr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fdpinkfr.html


<!-- 参考信息 -->