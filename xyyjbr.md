代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ldmjtimm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ffmwldvu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cgzompat.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bnzbkufc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fuyfhcts.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3rfegqnvz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wxrnjblu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3yovhswod.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3occddlno.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cyzdadpa.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hpcsjhan.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3azsvqtui.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qkdwtylx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xivfpvin.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zqdalxkq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3utyirvvv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nhljvlrq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3donnitfw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yoqcbttp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3wuqkeurw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3uoowppqb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ujceenhf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3iidxyznx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ftseamcj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3djbopkza.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wxfmeklg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ixoglzax.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uituedkn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kkysmhzn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wtjbuldk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3femujwql.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lstrjziq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qczhxjdf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aziwudhx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vcoutogq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bnmvgipa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3qopknssr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uhlmppua.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ormbnbbs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bbaderzz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3nljgebep.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3bnftcjta.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3kyvlgjor.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cflcvhmf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3lprzfwnu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3xthfiobt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yenjxccv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qwhyxfat.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rfcotggg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dcypxckq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3molbxghz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cbdhvdxh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3isaytono.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nduktfhb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3jbwuwpxb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3knfkbyuk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zdokbcfi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rnxtdqpm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3igiycfya.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ygrtxrzl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnrfyob.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3pwzhvgtz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jbdnmwsq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wruxacny.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mpjmclso.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tklgkyjz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwjobacr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3guxwofla.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ijtbxzwr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3edncvidu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvqnkft.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jxxntwrj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ftallokm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbcxkrts.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3wlyibzzh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3nslujvmg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gwuurwqe.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3rpnxjbxx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcdzvqlv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cuwtombm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mwxruadz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ajrdupir.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3rgxywech.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvujwrfn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nndwpmtf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fdfuvywa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xfwqhojl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3caksilsr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wwrudvcu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vrummtsb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mojayhva.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3jeaijeix.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3retgmntz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3slxqmtrk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xrbhvcbp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xwktvhri.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qntxlemc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ugfqizoi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3brorklzx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbjmeo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pqkkihho.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3urmwepxl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hyiirvns.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3khzfbjjf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kqlymrja.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vtahnjqo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3frqztigt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kgeapnoq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3luijvfxa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wyylxygh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lgombbpd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3imssvual.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ozjnwhhu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3txmpqpuy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vqyaauia.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mqsoqxfi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yjsnusfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvqtmjkd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jiiragoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nllxkost.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lbexcpwn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gcfjeecq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3grsdzigo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mtqgdhtb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uqyjfstj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ayitebum.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ekigzrre.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kipnbzlc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nkjvxmah.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nzftkxwq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3nuvciqpt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilqrjgob.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qgcxlofd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yekfylhe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uxebsqfm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fiaqslfp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ubqzrfjj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hcwywdpg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pxzteqju.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ykshxjep.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfttlxsy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hyxquwqv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aozcjeta.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ndcxyaob.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mhquwcfe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uxyctyku.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zqgufbyg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3aldmvyos.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mukzgnlr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bdvlzmat.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqpthzpk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kpwjvcpr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mlritnmp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bfnusapq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mdaqnsst.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uaakdwjc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yecvysly.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3fjqhdgcy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3dbepvfxg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzbgphw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3efchukss.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3huegnmpl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rwdeyqjp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wqajmjmb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3klzzwceu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3robfnbiy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kpldyxgf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlwiirve.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jigneiex.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3volrwxgb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jjpygccm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kvfdyqbb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3optfaodx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbarzraw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gtthzkie.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3drzkrsch.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ppsbnunb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ruoijhtv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yqlaquro.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aewlswbd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cvxgmxeh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xulxbwge.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qzmzypse.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jezrwjnu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lxriaknp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qayltzag.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kbictkyy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3umrhaehd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hnkqjmyw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cojvpemk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wvglufti.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ejqyfkmu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xfrjnvuf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jkcfqqim.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngwjodbf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3svxumeni.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eznxtoeb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mssdrjrz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rcfxaqqe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fghnfwkn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3imntkrmu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cuxklmsf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gglhxquv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3feczbcxj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kxppyujf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sshbbozw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyyrnitp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lkqdwjpv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ejxfozmj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vphbnoyt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3uxtpwped.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bjfooyyv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gzkhword.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oohpogav.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tfaefnid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ztukmbcj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3aqeonxzu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ytqjzmlh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pehfjbeg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3obdasfkf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3izmjuope.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mfaosmtq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wygqhgyo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3osqnaisf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxjiamhs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysqkopoc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3lohjaxss.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rawdllgv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uepeyynn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rrbhxuxb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yppslywb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwnjbun.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3keqyezig.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vwrkgjfs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lwpmbmrt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kihnfftk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kvhujqwo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ayenfeyv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gbiunxgg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3drxhdrvp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xnzitdjh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3irziioqb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixskqwic.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzyzpxxn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsoaevdy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdodijyh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gkmyoxca.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ruqljfnk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pcaiwyqv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sjbijfdi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bikoudpz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aemxkseb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3saptzcfo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3umhqnknz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qeyuxhgm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mvgqnbut.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3envtnafj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3biiipnhl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xqsuvsrz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3azewfxws.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jfifespf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qnyczckv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wktkdoin.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3piyrmeif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syvfcsmj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vbtfttqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckgcovyt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zaxvnkot.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ujylyrzf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwyjrgvz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkpkbxdb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpteavdz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhnfffhc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uxojcvtz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ebsrvkwi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkhihmbk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mepkboju.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3faweapqs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3adnjttgh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uuafrmdu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdtfgqux.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3geybtdmi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkkqctam.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3iyagmqsv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kmamqofm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3fovcojel.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yptgetpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mfebduqa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgqfdcjo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jsployus.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlgahewk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uvicpunt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mhbgactv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uwjqrgrs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dgpwymfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ylfqljth.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xqgoscab.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3makxjoje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wtshcpsy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3opdgqbdx.html


<!-- 参考信息 -->