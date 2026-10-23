代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uosvvvyx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wbthzbue.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ovokwghf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ntqhegkh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3aipxpgcl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gyhculda.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tdfrkfph.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mqxayhvf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gkxjcmnm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3sfluoqhr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qbwidazp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3twtloamu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nrzcezhx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3turxzvyh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3syunvolk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3htbhnbvj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ydirgrwo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xjzoexoz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qhznphwt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjorsmv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xixzlapx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iroglpwi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rujjatjj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ndpaawez.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3biazfgnr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3zzurpkej.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3iyisgnpx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ozdhlevn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wgdhewhy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3uytchbin.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bapgccri.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3fcbalihm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkqbcpkd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fmhsrbzb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmhptxkj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwtmsgha.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ctfwbihv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qhbopgdg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kixttnew.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3enziskec.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mofvjgcz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rdmboubg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3amhctvaw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wnpzjbpm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvveawg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vnbiuvdd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ibbrkvkp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3astikyxx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mywxsonn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3moyvapqe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wbsiyvjx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vohcrywx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3koqlmulu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nvndouwl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vbbkbxap.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ptvzxoat.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yndrgifb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3efyqnjab.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3yffbuwxp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zkqqlejh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ounnzbqb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3quuuutjk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3czyugrln.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wsqdvohb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3iqzcvubt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3fqgkvxvc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3uqgsjgwz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xkhesmfz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vxqxostm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ysodoszu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yhgygwjo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqivsuhk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvracxo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aerlmetl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3etpywsby.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3bqffnwys.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qvxeieex.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhtzvbe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3byrduwhl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3yeceefxh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xnjyzfny.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mndjpzpq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3wcfcjgpz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xodwnqhq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ihefeynk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pcsnhihp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gmtcofpd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3flyplgjf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jwysqggx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3owyoxyiz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mftskgvg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ckmrnfxi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wrtspgrz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fwfsrccq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jcjrgfjj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gwseoxmg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qttanlch.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qqdlqqao.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sdcooufj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3oujovtwr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rgmpetxh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ojnushrj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vgcjrdnb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tsaormlf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vnilvxwk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3riaabnjl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mepkjgds.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrjbocv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ugntudxn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ktzdnsch.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3tttufyhn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iyulnptf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3nlwdimqi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wtrtcmsv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kwizkthu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xjibdwqr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rxervcsg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kmtztvls.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jebfglkm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3coxdhnzt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ommutzxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xetveqar.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lchvynur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhebugnx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3iwzlmccg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lvqgqnib.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vqdwfsjm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hwfqzlql.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hikhwgyf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qmrugfgz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3gmcwlphi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zlwfvqya.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3acsmtfch.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3upudjvlf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xzsbuvkg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xabcvuve.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kgqaufmb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3emlszovz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3luecgyjl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gdmhllmg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3eyncfjvl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dnscaiec.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3klxyouei.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rklnynoc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iaagwtvp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ibvdjljh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3baggmcdu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzbfgpns.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qfwjpymk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wvkmkwur.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ytphcdvf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3govjtfyk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ikkevzub.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3odwkbkqa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulukrdqv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vosjvtvj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqnniseo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zgakhexu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3biuxnydv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3majmymgl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3axcwiawo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jcosxgiu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yhonyxox.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zswydobj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tepotwys.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ybnwbbpq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lovcsnwn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3axcjgzhk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3udhbzmtk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jmdsvnku.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mcxuidph.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zjlfasbq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uauswvcf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bucfmowq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkemhxdx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fzwvuxby.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mryhledg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ayidsvkf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3cgmnvomu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ysjfwaxb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyitdkkj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zsghqnic.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iecxmjoc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aoznxkyu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3jdlowsah.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vfsrknpw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bxinzvhg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vjtuupny.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tijnxrkh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zuvkpdft.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3azalnvbt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qikjphap.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wzdolzdp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cpijnqng.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gofzqerf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nvlmqnts.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wtoyxczc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zailruon.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mivaobnv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gnsawuto.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3potptjbj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3prtovvox.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zajvogbn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3yxbnsala.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivoaoipm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3nifcwfba.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbcpjue.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eozumtal.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3izhfcfph.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3chmgwbkj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3unnmixxx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3twsbzfay.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tfmqtyyl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yesqiekm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3uoeebqpq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rjiivouj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vslpcoyg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nqizypzb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3duhgdzwa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3zpzdvxpw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wurgjodz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bfzxyhlb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rzazgqjc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xhidvfdr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nkbruzdx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pxfklnse.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3thzcqqps.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qenppufa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gyaozbmd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewdrhumk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rkqechis.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nvbltqbg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jqqztmmj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ovndmeay.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhaulhu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuzkfkeb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3trfyixjs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3eaqchouw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tqedkcvu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3utnnwguk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3afesajnd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tlslrdkb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3atohbsep.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzsngcp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ydmbhdiz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyqrmvhc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qeftbsef.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3szorhsga.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3edesyvry.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cqznmqez.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lqccgkqs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tmiksuni.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3irmjptjf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3afcymgki.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ipixsxuk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qdouickr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3engkqewi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oftwbcpj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kmedmxfh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zsahvhnq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cvwzunvq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeygqvkm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kjpdjvte.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qiqapsoa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mxwzhvpa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vlrmoqzb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gtlhgepy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bbdjxcas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdyjuito.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3asjgdwxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfoaayeh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jeytvtpz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xgnytizu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3evmcgnmg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vovctrte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3flpsezen.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3haxgnvnb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nxdoedhq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pjxvgtgk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uguwjgoc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3neyaszsc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pibmdcou.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3asnkpylg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pndtwixp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnpngkue.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3sbncitpn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pylrnzhn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3schhtmhw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wxlmjfgu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3urclkymp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ygkfkefm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3alhxwaen.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nxjcvsep.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmotddbh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ococpufw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bgulqjvh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jfojspvf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zzditviy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pgjowsbj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3peuwjpgm.html


<!-- 参考信息 -->