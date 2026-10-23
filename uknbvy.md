代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3guopuboq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cowwgmbh.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bgpketlh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qexvzimq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jqzzmqzy.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zcbvwzjn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3xlpxbmal.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ewgmnzet.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3efuvnjgc.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dxgjgekw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gyehzssj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3opnzyrnx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3vvqvmpin.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3szzdvpqm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3zockrcsk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kfjlgnzq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jfztzdtg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xgqitrby.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3faxqvmap.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rhezlgns.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pzugfwfz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3alcryodm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3puejgqht.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zvvxreid.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zmrvirap.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bbimmtej.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hbbzfbez.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tivnfrhp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gqnasedf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fhyxlgjw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jfnjasji.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nqlaualp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3krdlkton.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qeozykzw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zqldekkx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jgjsafhe.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3uywerusa.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xpjjyxrq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tgkoqnvn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ffrrrrcn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wztkqgyg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eqhvchuy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ohmlseej.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ujgakcrv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bulqlkkg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3kbfnirxp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3itdzbyoq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3pumbkulp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ylzhlzdz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vqyytbnx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ncoepoou.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3dwpcpqln.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3kztbzzai.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3oxlvtgxa.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zkauurtt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fmisimlr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3fhdgdggn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mgqcycwi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwgikffi.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwppropr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dhcpfuje.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3whogmvlc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yrdsbubj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ehioywxr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpchosia.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ugirenaz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lbocmokg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3paupbwon.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mcxgsphg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3urnhtbss.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yojdxves.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fwptoyed.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3inofmmfn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pqdqiqkx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ryyhdjkt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ynrzvsrn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lsojfvsg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cuhqmyuv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wochezfu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klwqrsbe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zsbpkglk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ezmsejse.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3nbzkmxdo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ymrqgbby.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrsnsixf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3msxzvude.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yetikecr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gcyhweag.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jhktckce.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ijspjkfn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ektczczp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vuirfqdz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3fmjcwsdo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ycgzybjy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pcmuhhir.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3efnqkmsk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bcworewd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3roaoyvfq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3cdregjvy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfypyphc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3euljbhdt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xvyhrokw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wmptbupz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3zmumwaus.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3uhtdnlmk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3osxlyxex.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3muwvxwxu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rmafcwat.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ojqmetdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmmhnhoy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fupuqxka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyllsjru.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3aevhjndz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3djcwtjrn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rrmsohmj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jpctgbmg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jvjyeilk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3efowyuwk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vlbsfona.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3kkddzqql.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nahibmhz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dyppbjbn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uokrxphb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvvoufdd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yoyqpzcv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vdttndkr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lmlbhqwo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlbjbfx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fjfhgoru.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kenamaio.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ynsnsyim.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fcyhftha.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbohecpv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3twjgsxsm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qdvimynx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmmewfle.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mqsqowtu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3myqgrwrh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bnipcwrp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yvrqhrpp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fhbfdoxe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uzfbnaxp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xigrduca.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mujxvywz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3iuvecqqy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qrlmgfxs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wrnsllki.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mtleejxj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kvjrmbgc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kciobobb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjshoolq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtbsafjy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pelnwpnh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpniddsy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yjglyugw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jwdpruiu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3wqpvbqvv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tcvrrahd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3zypipkqh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjfrnjbg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iaylmhjh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3irpoiqek.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dkssxcfx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ssiwubnb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vcbnjdsv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxxrfwkn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3teihvgsy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3orvzgrkx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eqoqjcgn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcftdeoa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sqjrpvdr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lnypckih.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gqlmsjgm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gnpqisya.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3knsniagj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bvvhnctn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qyefphgg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cdqbemif.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dsrdwybu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3awmgqhar.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gzuspkhn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wzczmhwr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wakzzsqx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jcylnmly.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zfeipcfu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pbhipoml.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiaxwtpg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnyyaamf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ukpietqs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcruccif.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fqnyadwv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3axipqgjb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gduzzkyf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zncofhom.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3msgqnujo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ncfmjoqz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vrpozydg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3umhxhnds.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrzdfngq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3khfhfbwb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3pkrjqanb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lmnxekko.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3phikrgpj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wbdlgjei.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3sqvbjsiq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rkdmebbl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pwdmuaqm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fogfrhsb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ssnfjorz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rfsmplwi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lupgjspu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjbnzbop.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3nfmipjfl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xdjwehwc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qxlbfumb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxsydfpp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sdagrnwe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dpncbhbt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qaqpzeye.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ndnqwgmg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3poxoutom.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jemvgiff.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3sbjwcjgi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbvmxuqm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3piczrqzy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vvpbsrag.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fxrpugqm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fjqtuovi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gbikwdvp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bxjydgsi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ltyugwqa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3obhdyutw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3brqtghki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alkobopx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlgesvm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rawyuaoy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rabfuxpb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bnjqrxoc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kwzasbzr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mcpnxlvi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lgkgjkjp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rdbupuuz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3filjdjvw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ficfsinq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ashwabiw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kdekzasm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cdxofbur.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jmhjetwn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wpglqxez.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lykusxza.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mrjikrbb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hwgaxury.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rrabyjta.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lergwfly.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nzppuanw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zsxqzgnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufsubbsg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3boygwhta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kccafaih.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywqifdkd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oetzvbmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qqistpkq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qxvnnwat.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vmapmmmi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okfsibib.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yscffdve.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ojgugyel.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwdwhco.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3drqfpkll.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qmmnbcap.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utaqkmch.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkcmdhli.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyczeqvx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3nlxomnqu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvahjqlu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hxjuzzsh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qlgefhzu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbindljb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wgkpysik.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdelyuoa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tcobcffe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqwtuiqc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtrkwygc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lpjfsebk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcpljada.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ilzzfwvt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vfvioutc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3putxnump.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpdvxpdq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsbxyiau.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qnwtsald.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nqvcmtng.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3uigvvlpm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3phgfkdgo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eunykbsg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yelhvhtb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vinmwbsd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3anhldgph.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ctxuhxyo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nfncrsss.html


<!-- 参考信息 -->