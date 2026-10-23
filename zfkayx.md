代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3btxnynxy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3psaijhzh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hogghsno.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3duicggjv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gwdnwsdv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ascqytdi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jilivpzt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3fapxvpsx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cdcdjdsd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dyjgbsfb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yacgwfuw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jfdrpxxq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zfpwooze.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ghalqqpu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gwcmrwmy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ejsemhtx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hzwbwbgr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xdyylxgf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ijycutyi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3nqaykbjg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3vyalnjqb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ezohlquq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybfsapdm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vzcpzkmw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qrypmupo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3dcxkwykg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyowujnz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3gwaulpgg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pkmudglo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rragwncb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3siahlxyf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wksyfecj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3adynxgrn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rzdmpmgd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3thnqmkyo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3whduecti.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3uenxquwd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lprrqoxy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3burtzefm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3urzammqq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vfryupci.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mcxuzzgm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3zaxgxaso.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3aqqiexrs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cevqrtaa.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tessxijl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mohkorry.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ewkdmdpy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pgkxrmba.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ysjljycq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qnpcjfix.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bmkfriaz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rsvzcyrg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nxwlledc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zwxjiins.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3trprhvif.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3smoizdvl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3cesdxmzk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tamgayjy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3icrcypgg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3cqpnsqod.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ikfatedn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mxipueta.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qubdnjpk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3khzbsezf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lodthglw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxfgwyz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3glroeohi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ptunvnau.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bjitkiev.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dgshwfnl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3hayhcqdn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgpermol.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frgqffum.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xdlvfvqm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xlokupqs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gglcgtls.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3dvqgnmis.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dilwqtuv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ynrxxdrb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3atcuparu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3piusinyv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lyicoymy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vvgwbowo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3akdiqvwm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3selxkhwy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sngkppkp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgxolka.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yoatjtes.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wbecdnel.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3egacvjzp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3djyymvqh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hxlcipsm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jpgpajjy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yeelqmmw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3wwuodvfh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fyztqrot.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ubhdsefk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iwrbxhmn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ugtgjshd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3smhbofko.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hsmkngmq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ogcdudgx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3aowllwjf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wtrsxknm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jvkmhdxx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3acbzbbgi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ysiswfze.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3omtokbqf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mgsulkue.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3goijcwev.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ajasasnx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rbhorzud.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ejskqbgo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yyjqsuom.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3remwvlwv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dzknwxjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vanirhkp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bgnvjgvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ryuufebo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xikxjuad.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cqvdhczp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3usermfhv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mixcoivr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ucvtjkag.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3taqokgmd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dmxqacgb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3emiyfwiv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sbvimqvt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vozexags.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jfyjdhpl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdjwrbiw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ulmgpapv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kmhbepzo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pgxkitdd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xtmratmv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3usxaxkey.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lylwsngn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3uuxnrdgv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hbrxwsbd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pjvcbvuc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovqttlro.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kguyvfft.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnrgzkro.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3houncynt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xcheevbm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3psmjkztq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uominwsm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rbfbnawa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hnhhlhbn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihttnuig.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3omiygytn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qoausbkt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3voitaekf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nejhmdfa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjtwirgo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qyyxnljd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fqtjfdxv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3emywruzk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrggdywi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yyewcays.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hqgglysb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgxhjgs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jldpkiie.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rwajxbmv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nmzbkjyg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zotkqsas.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwwbnln.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmiugbn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmdotkoh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffateisd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ohwugdvb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3stnyjbgu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwhiwvfk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3naubwzki.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cxncswgy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjnvsfoz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdvieiqw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3omolfcyb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljxltqvk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ikgmkvgt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kxxahfal.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zqjmxlte.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fxtzmtrc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ivtzhbhm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wsnsxdoo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oryytzhk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rsblpvau.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jdpeojip.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfktoatx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xtgijmde.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtootku.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3nnxnoesm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jlxcmcma.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdiyoda.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ksopjavp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ponydppz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ogxsgrpa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3npizoolv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3agdovpdk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ezdttcgq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3frhoqdcm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3iohrbnrj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dzfedgts.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dfmotonv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mbzxmmcv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cjhgclvm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kaisqmvo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hvqtvqxg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oysjupzn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3foicdvzc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ajtrvdnd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ixycnfkb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3klxvhizf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3debvlcsn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lcyveyrj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3foixtgfv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3svrruimi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkwqlgt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cnkbmwei.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3yholybxz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vkzltueb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbezxzh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pjgkzxom.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sbrayqzi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uyrijglz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3oaicmoez.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3uorxfonm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3akzcrhjp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ymebxnoc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fgrebkpt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ojlqiqbd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzptwzqt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wjiroali.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxiwlo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tlgkicoc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rozqcnws.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rcabumzy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jtlnboep.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ydgpvycn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xplrofhr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnzilvqk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3srvmxtrk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hmtlxtpr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3unoehuyd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjfoxoov.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ctroqzja.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3aerlhawe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zgmmmvzf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3twbmjicd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hhopwbnh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dgiangsp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3llwmcmol.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmmoeyon.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nvfwilfd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3buaffmba.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gjfxbntl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmufbckj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3siaomthq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xniiczqm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jscaibey.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fnybolru.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hzddlnqz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gexbzmec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qabbrqxd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hbunakgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rezmmvab.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3juibxeai.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kgvbseop.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jnwxhvco.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdhhpxfc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3anvtkssl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hazugtbz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdixzfu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ksfwcgre.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttpiewmw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cobbolhp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3blxoegga.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kfqtsree.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gzmwconv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgotalpl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ajegsjyo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkyhkjjz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3apacvauc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mgegqyus.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tohvuawp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3eqooyteh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3anjmvjpy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yrvahcqo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uneczzhv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gkrusunu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3methowbe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hjrlafaw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3aopiaupr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykbqjgfx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rsccdjjz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xlixxgtl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nsfxtdln.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cqmawcan.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dlyuvsoq.html


<!-- 参考信息 -->