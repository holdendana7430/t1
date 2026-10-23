代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtpnrsx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3iustkfrj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zicinbty.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nmyxophz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lzbqrnkg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wupwwmdc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lmjculcz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3plvywnuq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cyyroxtx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zozbukpw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3pwoycmnr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttwbdsnx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dwxdictt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nskxylpc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3afasbbjf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lpdjujea.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3eandgcqm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ebqorpxu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3alamydnl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zvkooihq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ufxqfroo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3leuvhfqi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rvnplqik.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixuqgcen.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dlxlkhpf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3prtgsfmn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lmsmudez.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ztsxrwtz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lobjbtvl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xplxfxzf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xkqajvuz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3csgxyqle.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vapfapya.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wumvglsa.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tikkrhwc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3qwxdszye.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ktkzonyh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3lujetkrt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uerdqiqk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gfsjuysa.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hmmollio.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cjdypigr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3yntztjmm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3fuvrzdxk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cnbnbgtc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hkpbzfwj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vkimzxcr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fequqffd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3xqtppgko.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3plzoiapo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pezyigap.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3jfervrxs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3akkjjgez.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3csfaxnwh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdynjlxk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rvrwsqes.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ywmgjebl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3igoghwgh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ymfrxoiy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ihvndhbm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hbvtvxqd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqefjqtj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qvktzotw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cbxugzvt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ppeomfgy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3snfxqkua.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3djlzvfit.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3iftxcipa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nqmhiakj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3lqmpjxvc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3monqodhv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dinynjdy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3htqvgjzf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ohuanoho.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jtoxldte.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3rskodvjf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ajobbllz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iqxtsbvf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3vftznjzl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3phufvxvl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hnfrvsyq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bfddywjh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vehbperp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3unmxkcjz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3gxegcsms.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3udnifmyb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jbdksbcr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vmdmsnbo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3sehqizvk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ywvbswhc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xldpqglu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3gwypyzpl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbznyxew.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3osxjrfnw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyxabhhx.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqyxdkci.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuoifmw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zurlmwzl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ubjgwagg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ndjkmnoa.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pvshyfug.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yybyzuni.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3bgitxzvx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lqnoenjm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vttxpaqp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3esmkuzmq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tggiyjjj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3myjmexuo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wdaoctdz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ooappaoh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xcqgkrdv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vekaqirs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cdgsonkq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3upiugwht.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qyozrkmu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kwwxeejl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3miuhjkzc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ehqqgptn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3tcorasus.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lufepljt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3wuihqwze.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ogqgroan.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jfhmdmes.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3zqyvnhvn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3orwrqpci.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ybqnkqfp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oylnoaqg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kfxqjfvn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3hjqcbopo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3jtbwnccj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujodkchw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqejpija.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dndhkwmh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjgxiklw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lndzntdp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xkdyhtto.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3lhtfrnhf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dcyhrmyj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3cafvjonf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3eqqockhz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qgtugwcc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qowwhiqh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vahqvovd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vzjzetpl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tlwuqfaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvorypuk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3gxhcjuiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iswciuit.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zaoigfzc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lnufgzsb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qkrnmrmh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oofdfgtj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xarsdhgu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fqiupbne.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ejqtjmeh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3afzmsrhm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yzzdopqt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ytinhjzm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3iamwkneo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcnauwew.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wmcsaukm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mlmmxqqw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zfdwxhmk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbpjnou.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3taoujson.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lipplddw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3cvskvufn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3huvpubyy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfgezmo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3omnxmbri.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3djcchlgo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ojlrbpuh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kilwbsqn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tundykud.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xfoctwlt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hgqlgyog.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3airpnrqn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vbastpaj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3agxzgllc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tnernxuc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iceadslr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fucxzvka.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xzbymcob.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxzocjjx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zrwnuxnx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ntdmcnrp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwscbqtg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uasxgncg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmvlqawe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3yfbjpsmc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gjnmklig.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3oucgrdpj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bzqsekhb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sykcegvt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ndaccesh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vresszqv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nqrzvuso.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3onxlijyp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vylffjyd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fqxktffm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jwaalgol.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vmloqawi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3utyowcam.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bhlijfej.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cdayefju.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrwxdozw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hayjbysi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bhykdxrm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fejkedaz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsezjcyi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zhqcwmvw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eookdojr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3iozevyld.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nqblpxzh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mowfnknd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fmzcelku.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tchlifsh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hjpyprss.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3itfvurvi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rzwjzpbh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gsvcddph.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ripuunwx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvsfxjoe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqkenoz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oihitoki.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyhvhneq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zkgrnvzy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qnkxuskh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gpchwiot.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3imsetduv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3xjyicuyj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3euifwbdr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zyrbupcp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dqilpdis.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycjdwvvo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sdvnuvsg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xailhsei.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zrvfitvl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3niqetbdd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uxdkoarr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xrpxvzrr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dvhvumyo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ninmdvow.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nopxpjgh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3acksdjwd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lpihnilj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cymwrclu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cocadjdw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jfmaoegz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xbyluovl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3suriyzyw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbbajdd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mbqelsif.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3oljsfezn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3thoitmrj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hgdjqdne.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ltepnmzb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ikrtrtum.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dygrvqbg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vonqncmo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qpquutlf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ulzducif.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mvqoqfwg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lksrwyoe.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qcjwxyft.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nlbacmtz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3tmkvsiny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gordumup.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xswvpjcd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3spfzibsn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rswmqojb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3iziewpyu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdyqjdsi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3spfqzfmw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lfbwdtui.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uhrojgul.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gnailypt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wqlpynay.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbkiivgq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oujcujst.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lmylucoc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fiflsmxi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tuchmghq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zxznknky.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ycgooeaa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjmbigqg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tvursoqw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wbcjtwrx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3arkakzuu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ylephpca.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3cpqdvhkw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dbevanfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdaenwnm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uejxdyyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubvqcxnn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vkhssmjc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lhnvttfa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cutrshgb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhsnxoet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yugxyjta.html


<!-- 参考信息 -->