代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2byhcylqr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2usiewttq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2whmntqbd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ximqivmr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kecluewg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2cphafhzc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kfqhupfl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ywfaawpi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gmowrdxl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2veinnvrt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ascxtbpw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2flkgugjv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ekilnnkp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cevbbxav.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jugjrgij.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2hdlkoubw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2epvszfsg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iwttwsxs.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ubntghaf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2auokvwgi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2vrbkakwa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xxyweaue.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixxabsoi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lshssfvh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2svqsvmiy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pdtxvjjy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvlsynri.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2eelabqwr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvszrjbb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hixqhbrv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2srjanzke.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fkyyucpj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuarrlxq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vrlouysf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2giuxjveo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vzxsfwcv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jfpjtrjh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2llkgcycn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ejtpzois.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wmehisjt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2izqomosx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2fuceofgi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2yhmplfmc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hpbrxthv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ozhfmdgg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrtfybvv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jytzekie.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2izgdifqk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zhknzcax.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rshbotsw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vkziapvs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wfbyreuq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gzoyjvyk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2kshxigil.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2sbgnuvzn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dpvfygki.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2awwcrkzo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tpymknnv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ygkdqbys.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gmiokotu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2iwksthki.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nylqfypz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2oqeopxbz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cfthntpd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2drkvmdud.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dqmfsgle.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcvdkkuh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pigvxuxh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ovvgjabz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbihyxl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ftcovljw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hcpvtpuy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vxgkhsug.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwumnyuk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2kklrcjoe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2oixugjrn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2sjsbpfjb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2evsgzubp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aycldrbf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2sapgrqxi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xyfgsuyh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pacdtsig.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wajaytjm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gdutiqsj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2guwshqol.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tbnqhgjk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cditzicq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqazxztg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uswebnqh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dlclbmls.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2cqvsqqpk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2mqblplzx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2msdfdbpo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lkvsusdp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xhdguuqw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zmxfvwhb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wgjdsnfi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ikkixuxq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xtfmcrnw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tmdcznig.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2lcozxddw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvikstef.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqbgbuob.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pdweekwg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zzrexdju.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzndcmgr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ycdycmaf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjuyjmds.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ymoaryjk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2aicvahvu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2slzenmdf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cilfzlrx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qsnuftof.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sxvchgvp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kcavvyes.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wwhyzlpl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2znhwzxpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nopccppt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rgqjiuav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppyrndjt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pzfvxjej.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kvqvghrr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlbzrgue.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ylrnawiz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2svssluuz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xipauada.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xwbrzifd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dlnotack.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yfzodkvq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hgwxnaqk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2sqmciamu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdoagqmh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xwbobwyp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2urhriyzy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ovfjmrgi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qtuadunr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jgqggygd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wkqyvcpg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nzizqfeo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2etmoagiq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vycymqjm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2czihzgaa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zslztydo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vomclbxa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2flxqxazr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2lvhvjubt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aknnjdlp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2njwtyimj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2futtudhy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2krxjueox.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxnixvy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtczhjjl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nvwmbfnq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xjqxabie.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ygriutnr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yyjjcekq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yfguggzr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgfhbdn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2esnesaiu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rklshxdw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aghgmxfr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbzxdlae.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2pnbjqblh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uyqvhzrx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiecvpvc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kxtfbixg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2sqqbwjii.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlsxrzjb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kfkhpsrn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvzidtsv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gaqawbmo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vnoakzbz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zynvztog.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fiawkhjv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ftjszczv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mgffnzvl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mtfnvbde.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cahdugvb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ridjsmjj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fjzamtip.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fcbflxuh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wzunhaou.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rdkuqgkl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2shzkesms.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2idmqrcoc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mtdbxiqq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ttkttbqv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2afhbhdyc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sdfvictc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwywnrc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jzwrmhzq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lwjmrefv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zvzcssij.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tpbwzhyj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptfbqrqr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvxnpknv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kvpcsrex.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uijmwhcq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpfchcrm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2oqpavlfe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qilipyeh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ilafanlj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rfdfqaht.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wvugzrma.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fkwblnkl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2diiqsshk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2swqmqkag.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uhaqkhdi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xblzqbly.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fwwyckew.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2czjvcwpg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2limfwfwd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dyqgdtae.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ohoefjzf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ivotqjiz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xmffdbuc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lmupzxmp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sootlorp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twjbwfod.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aatjryjf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qxnucmbl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ipqafyxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ycwldsvb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yiifkhts.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ffbmeokg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2smbjfcnx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pjbepnbh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zsmppnwe.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ihhlcxon.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lcyvevgn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2abrdccqk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hzvkijko.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gczsuyzl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dyppmjbc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kcuookzg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dwuhpqov.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2oflckwxd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vnbotssz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lycstcpf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbznqft.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frkzjale.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2phordobq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pbhreiua.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmaxovvj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqdzwwby.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lufpmsio.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jmrefnap.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2sezigbid.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wcjcippf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wqfzbwdz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hzjtshra.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2woporjxs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xkwelgtj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ejrkkghq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fdudizxs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bgbywihz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cyxhbjdh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjobchlu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2szcqudlu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vtkgmxve.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bfhwpbal.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2etxhmwjy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wkahpiwb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jqgichik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukfenlhh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2btlmwlsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pohnklin.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqtphulu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2csqzviym.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wnwgxawh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgijybnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crpduxaj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxgbqhaj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oaihyrjp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xpjiktbb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2obqgqhak.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fvgnweqs.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2diayqktv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zeqursli.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppdkntvo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awhvelvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vvavxnrs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ycnbmkmo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rchitork.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kaqnmaet.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rsjglztf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2slestagh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vsdnptav.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2skbsrthg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yzozjfeo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmnzwvaq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fokgulwx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2hinuudrg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fsalwkhj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2inpnttcd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ofzifflh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2aufekazt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwusjlfw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2aykvjsot.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mpwijjtu.html


<!-- 参考信息 -->