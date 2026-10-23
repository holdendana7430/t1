代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3httqwuhg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3rbkvbieg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3aoutmaih.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dgyxijvf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3olxakfqc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggxyhzqk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3lbvldnnc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ermymqli.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3spbsvlis.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3jkhqhbrt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3fikwnocd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3klzidvbq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hihougdd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tiyopmpv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tetoviqr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wkyczeza.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ekwinrdj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jyyqrezy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3khamdiqi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlcfgjnx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bemzywed.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zsodyafs.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eafpfpbg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3yspgjugv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfbjxsq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3skmrmbac.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tzcfjbxk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dyoyxilx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jvkpghkx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ualgkdlf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ddwpvwvu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3isgqxatw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vgydqjuf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yqhlxnwv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vushltri.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pbewccjy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xjoiqvrh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3mlrbiefw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sjgcildo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kchidsfk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vqlttgae.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3fatplfmx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dmzalwjf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jnyrsbej.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qjeohvxm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cxjqfubq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yjtemwli.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3erwbemsx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zoxskyur.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jvlqjogp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3tavkumrm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3uoeeqlzi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lwfcjxep.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xaulagea.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gidlkkzl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nlicmldb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3yenjvhuw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rxmbcskm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfaoloun.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvlkvngs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3fsmqncyv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yhcpsenf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfklkinb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3cfvrroud.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dwxiuzdx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cgdtdkqk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwcwoxas.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sbuxhzpy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pguinlud.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpostngx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lwteuzqw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gbawsrym.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3bdkeoeua.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ihnjefgi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gysrceaw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gudmwsej.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3namjosxd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mpepfeec.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3fccrmdaw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ddyqisun.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3logrflaa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjlfdqjm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3znymhpin.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kbiicpoh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3buqtamll.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3socdoguy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3spyeblcu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3utbjjvge.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3czirohrt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rmleixae.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3cujbfyyc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3agassezm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xgvtjabm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3lzpbmiwf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3impnaeol.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qqhuorfq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mozovhys.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3pqcgiuzl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3nevmytql.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ztospfws.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zjbblkue.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpcbibq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3evrnsvcs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjsimrea.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qeqaxrue.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kupwwwph.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qibeooma.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3klrcbpaq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3olfeomte.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gduvahxk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3klcwpcog.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3nzsyhsvb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ogbgkqzp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nruovujf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhazwndv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jsmzlrvg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3tgewjccc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bwkkcmyt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hmvbumxh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nhmtjpov.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3epaekwun.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wunjnxqj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dfrbfauu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qcotsfah.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rbshgink.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rpaqhdxy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wtwblspj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3oklxupmp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bpmoksjk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zybcrlba.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zxxisbhe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3sqjbqkpd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fneaesak.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3kzmiuezw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jvkzrczg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3higsyfip.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jkwfujzj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eonmaswm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3agcwfyyx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wikzjffi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcppuugs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gdukfbnd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3oxjseslc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwquxnlk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ecvmmwhc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3dallvosu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3dsoaxllr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jlpsvqbj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dsfpvnnv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xnpgmzod.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3iwmgoghv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wkijrexu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kcufjijr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snzlqjyf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qrorjsdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywcbuuot.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3nayuifjk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wjpijsjp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jwapntdy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ujaayvws.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eikjaecz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tvguljqu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yyuyshbo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3trxpqers.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rhccvgaa.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3yglnlqzo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nyskpizq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkqnxtuu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xtxlwowe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qfdtsifm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zkytxkmn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wqmhipuz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ofhmowtf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lakskrql.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3evnwzofm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3scybwqyt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3errzyucp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wswjueae.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovgfphlo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xvhrxzjy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gnmjmkcr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3jrcecntd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fbskyjhx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bfdnljvy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mydxehxg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kpycgopz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqvxdgpd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mraxazfa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zarafvby.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3eixusrjp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3alfukjjy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddakstme.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iufvpaqx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3isbusmkp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydgkxfod.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3svvemhik.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qpdfgkzh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3tjjayyjq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfdtezn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bgwhzfsf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ypfdkbih.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nadhptmk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pkljnzoe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3oxiucmya.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sptkkipc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqouyqsu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxpkwaqz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pdprxrqi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3smwbrvhs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dknhyfzg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3roiniqoo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tgzhwupq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jecpuqax.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xoxbnmyc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3exzpzoje.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tfkyarsu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3iirdtcdl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gfaykvzb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3metctydn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vlttzhkj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qlbtagvv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ioodapdt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vazwjjcj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uygtcxwy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3djwyajbx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkluctgq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jhviddhk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sgqkxlyt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3nopsosqz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jzvjhlsb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrwurvyk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyrabbpj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gwlsecbo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxigaqdi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3neufagys.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qznzuhas.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebyrqenx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dvzvftcb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lkuyihzb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gychrdlm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dbflrfij.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fpeqpneg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltbzgauh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3psfxuitp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nnvbljog.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqptouyj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zqitkyga.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vobsyfix.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vbkoahjo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pceqbdka.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3igptfjxr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lmpvtozm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vbewkohr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xtcgeang.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvqimbp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3danwrpww.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3vbhiakpj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jflwfqsa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bhzlthii.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ofeqgyvv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yjdyfzkq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xuyqgfjy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nuzqjcxx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tjpjzlli.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qjfxyvfy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jplvrvli.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3jredzzhr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sqtdoacp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcheclwe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3euaxkvli.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ibokotif.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jkuyneyk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lwcpagal.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vexmykcr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zfnbwjyo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3whprdgql.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyadiqlp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vnrydvfv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrkjibb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lijhebst.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ovgrldiw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctgsnkgw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fwrkqlks.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xakvhhec.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ltvkzzym.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hleclnic.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wuqzijwh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eyrzjwlk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eclnfdig.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wwatajob.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xaomgnqg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hrjwqrtv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ewtqzqlc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hqsmhrzc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3swbsqnma.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mmerwizz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fhfcjjvp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ysujohst.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gzzeffgi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vrrembyy.html


<!-- 参考信息 -->