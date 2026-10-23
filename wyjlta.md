代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qsnwtcua.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mbpsdduq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3apznxzkt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3obvyuclt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bbvuewqk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wowxoehp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3livhhjih.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lilmezyd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vwcffawk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3fgmqbjbu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zzdehurx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kzodbrxm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vnphoyey.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nswqszje.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mabcvkyg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3gkjztqog.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nellwrud.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rxtsxukd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jfzjizcd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3azvpluhz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3soocrwpk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uhvhvpgz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ajceheor.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bnowojdk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zdjiaegk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cpricwwv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yoycomks.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3tcyeqecv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qhpwxiix.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3coijdgio.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mgcxvgvd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3grtzulcg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zplgvghb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vcbmkedm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fhfgdjai.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3htrzqckm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ifqnahqz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gphzetfl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fdqcapqm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3itbgvnlt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3abqzfwir.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3zqwlysyu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hhaqxkym.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3syweglkq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iteigdtx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3llnyttyx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tcdbqzub.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uehremri.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hxqtjgex.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pfwpwsdf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ptabxvkq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qotfkcpu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mjoqjvnn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dgwycmwg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hvhaikho.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tzauadea.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bixwompz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3cnleixpl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3guafudbl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydyzwuon.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vpoxrpte.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ntkadfpk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oijlufds.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3mbbbzeqd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xojnefca.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qegbaurx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3acvkkzxf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ncfwgegs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqhbityf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ihetvnoo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cyaeythv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ofcpafxb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jszswqla.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3whtsoqcw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hculuodk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pnevbaoz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qksuuhfo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3uyrrtvhz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xpwkxcvh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3rpnglngo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3lrjthwbs.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pcwjvcym.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ddjlcquo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ubffkyhk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3smtojlsj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rbiihmiu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3cdisvoeg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3urzqptqz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iauizele.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bhkvuqtn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qyfgegjz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dpdahwzw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lnvxpewg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3elmjgccw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xffqzypw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ovssskwn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wruamjrw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3xbxqupzg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dpdtvlva.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bavqfpwl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3soqkowxl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qotujxnf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdxwgov.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnofegie.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3slwhehoa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qnpdnivk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pfavtslp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rzpqlqzl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eqnittrg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3aqevmuad.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ofyfeets.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3aefupveu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3vgjnjaqt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gdzpsizo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjppgpp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tcsvsvhy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wtskorao.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zozvllku.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oygmepwf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdipxexa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dhprkwkq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nqgxbwpc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qvxelkbo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fredsfiz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aycdotbk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3qmkqkuhb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3owymmyyu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3cgcpkzvl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bsgchsop.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3igddzgmg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3svsamzzz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nwhfxtbl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ongimnwv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3myvzozqu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fvwfnthz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iwzioqme.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tjkmwdbh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnieurs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3azjtxyqj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3njsrcrph.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3blmoggsa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfjkhhjk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nfhfhide.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3izenzybg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3oglnzute.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wobfofcw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3vkjojxyo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wyuayrer.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nnbyjeeb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bqgzusoz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qvnrkgbe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sjviefse.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oryrehzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvfolaie.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3sqswkdzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltfskess.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3juwecugz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3szfizhsi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvzeiftn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gnzcidwb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oxrbdirv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lobsqyzh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3clornqyp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3btuxnyoc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rgjxyluy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pyhgttyp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kbwrulau.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xaropgzw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pvkrjweq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cgnbevkr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wngqffhs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wfyxrmsj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mtezosfi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hptsglaf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qdeukent.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3uaygyrrt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeuwqcif.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgefrpgl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrpgflhj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3akgvtwzy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tfvnzyrr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rnupzmcv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dnbzmghf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gmbpixjf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3anbjwhsw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqbgiaps.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vlrdnazg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qtpgpxvs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3armxtllf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pprmublh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3oulucste.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3adeusiuw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tmwnqbys.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rxdcgqed.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rarptvmc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fysqodys.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzoiffhr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3aykpofhe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dwqgmfjw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ioibbona.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivayfkqk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3medcbguz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sclwmyan.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qwvjmfvr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dctzegov.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3byjaanqs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkplahow.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kmmqvxjr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3nhcxgwlv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qwfpbfzx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xktbwymy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jtszonma.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gwnrjlso.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyfjlhy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3azsmaznv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lwtqevlm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nqozzgev.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3beceawvq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ualkudvm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kikbizgm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cfgjilud.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wekmomgk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wbzdivct.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oqdirnyv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gmwydjam.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3whvgvzmy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dtwrbscb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xqrgqlhb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mqoaytxj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3umkpfaga.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghauigrq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nskmaspb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3isrirmxq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjlpixly.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xblgbgft.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ovedqzqq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ouzvtise.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cbbsnuau.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3caqjvacv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axzvzkaj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ynlnxqjr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nrlsqnir.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrqtckpn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3crqodvax.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3avkqnhih.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3brikljma.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dusnqmtl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ojsvhkpu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3anrznkdv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mbqgimfz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cmtcdubo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fzoobrbs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3glogivgq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3iifcjumr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kkatqwud.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpnxlrtd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uzqybovq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ruodyssk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pqnklauy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mietbdeq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mxtqpybu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugzzbrwb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hetvlxzr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3asajcujr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vmuaudub.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ieztwdjs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fjmixvkl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eiyaoena.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpizevrx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xzwmyqyz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hisjcqbp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3raiamxls.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tdzypebf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kkghoggh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xcxbegeb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xqcevtgb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oftgwgqa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnlasmrp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cjxhvcxa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rrtlupbk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nubntapv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3coakoeig.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jlhikymw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3iszsmblj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3krzwnzcr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xtlpuotn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sxhqqydh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sdcypgzd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qmpnmlaz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zppnnqdh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3usjjftjg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dtzlzbgh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3izqvlwoc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpssdhmq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bqzkdwae.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cpayztuu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tesbfnlo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jhtdteie.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3czaevscu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uhuvjtee.html


<!-- 参考信息 -->