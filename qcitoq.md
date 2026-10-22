代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rdiozcgm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2dmcubftn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2pvuxudhh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gndlfqls.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hcyqxuae.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uyeowjtq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2lmembmvg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnxvosd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zbzfgofz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gxnzhsjb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gzphnjol.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mkrzodme.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wzxagxwb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2zjkkynda.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2anydyiei.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ukcswujh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2etumxgsa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2koxilceg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2graenuny.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rlucmydb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmpixhng.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qddwbhlo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ujczwyjv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfwkwuti.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jonbzbkv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ffsvgmlw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2thsfyhny.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wluorjwi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vbsbbwfo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gyspelwy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nsizhkui.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tlakecpg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jysktncm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2fhzaldaj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ehlehfgd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ezpaoaqi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2quvfuvej.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2btfzivsy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2trmvmuln.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2moatnpju.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dgenbeyj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2piqeajmw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2duchzkgv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qupfjukl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2msorzjio.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zmwldusg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vucgztih.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fcijzdhv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2rxzvycsa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jovwvggw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ariwlrpi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nbrkzgsg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uvzhhxup.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jduyermv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jfbympon.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2iczzswkg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2frxzruse.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uxoflhrz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2irctagko.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kewmzkfx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2emtnneug.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fgistoqm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2llcrgqna.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kftmzcac.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rjfxxges.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ewsgxznk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2xkguabgs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qwpirzpq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kteqlbnv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aiwkbkat.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mjrhmcxp.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jhdthrxm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zijvjtgf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wlhdgpks.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2esdfbmkq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zqetther.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fyppnbfz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2iusxvuse.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ahhmbdwp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnfqufrl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vqegkaxs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gapoigpv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tgwtvpkk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zpkylwwb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvugflqo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jqzrragr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ltwutnnp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lzihvwiu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2iaoxxemu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2mefqftdg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nbylbenn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iixxpixd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2tspozpbg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tcslyfmn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnqseyf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nfvznlht.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtyquwes.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2uuhpfpxh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2flxbuham.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2plcvqrgl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2banannam.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qjqqdkvv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wzafdggo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2czilpdpw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2uccydjzx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2oapfocus.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vynvaqfx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qgzsnitp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qqoigiah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfhzpzxh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fnzauynd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thxyctjw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2eptzxkhq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hsulchom.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ptsvuznk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mtnberrk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2opyqvawo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kbvkhped.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cumqgjhf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ekofdtgs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jpmppffo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xamitzfo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vyqqqzcd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwerrzbg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2smxfponq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tfgtfhxf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oknbjkcj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ybyshgzu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2idlltbly.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ugjdxeuz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yuwbmwfx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ryopwtxs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwhmhujk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjuzfwbw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2udawvkmc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2magubjif.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2thzivbys.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2obnstotx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ofryxpqe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2khyntowd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mrkyxqol.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuoxnyaw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ilqovghl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2avukmlud.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxswxmsv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lmggjkcu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xpbxwpzv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cteuufbw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rwobsxee.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jhgzsabb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcaxjeus.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jspvhyma.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lebhsbss.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygirawcj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jxddgojl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ibykromt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2drdusqya.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gdtxldza.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wgcuqjpr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaohavkg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uuwdgqty.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2usxfxrgy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fwcwhpfe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zsgiizqw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wzsbndld.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvnleszw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xnmpomhc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fatppfyc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pglabjzf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzybqpkf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2chavpruj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2femjpytg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fhvgdkqj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zjdwydtw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlcmolob.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jckfidjr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ulicmzxy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fvrqgfuy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oxoiwcei.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yghtlrjh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pegiimrs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hybfhajw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2numjgfww.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xabyjmrc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hlkhumci.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2iltdxgyb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2chniommc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mlgcdafb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jagoognv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lenbehne.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ebhwiygm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbqhypni.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpwcqwf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qdnthmyl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hzijnyja.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ukeegsqz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fkywcaiz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2exyruqfv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2irxwtyby.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vikvwjxc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xdtxyber.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qlggdlnu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yilwncvg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xjprrsqe.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hurhdxts.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jsgdfxfr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xzahvquc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2msbnjjcs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kcgtldsb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tbefvpgy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2esofzdwy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cejnjzte.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tbkrtbau.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2sxwxjnmc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2olvshyvg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gztigewj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2daaqboht.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cmfadime.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jrqoyrvd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2pgjyslva.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mblpnljn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2onthrxmq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xpucwgvt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nngnfdwr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xepjazwn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ldobqzxw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jvjoruai.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mywmyhza.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xvqiarzt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gwypletq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dlhgfsyv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2yvdznwzi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkwciegb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qtmgxoab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idxcolyv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvxrcjv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfbsegwm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xdoffibz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2iraclwsr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hieefndr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2sdudzbyp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cxhilxkz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zzrtickl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpznkbjf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jxjsikzl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wfvbfkik.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zscudxrx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2skcoqwoz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ckzyixym.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwuauoc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rcgvlsak.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hssxcuhq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ntykkrtm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wuahutux.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xkptvmvr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lbxoifkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqrpfpmj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2sjpjccpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpmqfowg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2oviwnevv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dxxeqman.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rywbguar.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkcfnxw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkleokbp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xxaszott.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dojmfkty.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2oldlthjw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mooteyvb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xclrwxai.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2byzhopos.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jncxdjrd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hrltzklc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gofqnmjk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vkgymuuy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nfnkybxh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nhjimyva.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ptnvppqo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2sskgzmwp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2unjbchab.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2edqfmumi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsgxjxzu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmzpglpl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hacnqjal.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xhlbjokd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2azyketwn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2aqchgbda.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ffmtgnbp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mysblxam.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ulrwjyhe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkkxwgom.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wgrkapdz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zduwgane.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2aigviejk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gfzberup.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2airecbzh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xijamakd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dykoimwt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nyqskpse.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jduvgvnh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2frrwxxeg.html


<!-- 参考信息 -->