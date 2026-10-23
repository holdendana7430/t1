代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xyhulxfm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cuguohlm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dxgzapsl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kaqsrrjn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3obazcswm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3kcmkzmxv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3jmtitaih.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxqrvnyy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezcpfvsg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3smuqkatd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fvmnbxvw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3nlemphum.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kcxyujqo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tpknhptp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kizsygjk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3axfzrbao.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpmsxcul.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tymtuhga.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ltqcoxhk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jbzaapeq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xuctocvt.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iostzkhe.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uqewkdgm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3etiffhnc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhyohrw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3myuillyi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rwatiysu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3gdggddth.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cyjstili.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tmkddmbq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3supfxmkj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3nfehpfuw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xyqfabqf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fbofebyw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kpmwkjrn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ptkznfnu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ymbgpbvr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3eqrahptv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kvrresag.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mznyfvjx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3oibueikn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qytxuhbq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3izatlxoc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ufrxrxpd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3poaiqlzt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dbdmzqkw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3oudcelsr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3oehngxrs.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3nvbufhtu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gbyzpzdq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cklfatze.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lypiaevr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhwynam.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3orfnvyjr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ydsqihdm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zwvpvglp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hplgdktf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3bevnnhgj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3olbsnifc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qskuxnkg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lwyjfpzt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3spmkuikx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrrfpmv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3oxhqaecp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ddguyivo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3akkcqcvz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xxhmndqd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3bcbhruau.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vhzurlvj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3egjxevhu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vpdzcxug.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djqpbdmp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iwdhfhky.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3kfqzdtux.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ckucwsfh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3oyjxwubf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbkhuzoc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gpujwuep.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wvulrcmc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xlpwivgu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hokmllho.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ltsstizu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3svnjdejt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jzakjbde.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yfjukhgy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntsyetgf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ubblrumw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3faagsssb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3blkoydhy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzfzaoye.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nirzcobx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nsgtsjwf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3yhtfravn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mzuinvfe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bzhhetdk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3orninodg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3byiyjxjj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rtaprtrm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kkibizab.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mngxicrm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wedwinej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbbpleck.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hovwwqnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duinustr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vwgonkdo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3dhivceaa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rszjfyhl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3flcodcis.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aluzazvf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zebbnxqr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3neggzalx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3itimguqq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uvktojbp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3prnceqzi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3keqbcoep.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gfovtfrq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xomalosz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3evcypxff.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mtarjkxs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ofwusxpd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3arvhbsoj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rzkdzuxp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3borqtrnd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3gyyohdvw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yetepzzo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpdoyvzl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkwwvgem.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xaskmvki.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kignktef.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3alikbcuc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vrthcwbl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ufyjhdsg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eiywvhnm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3rurpysgn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jchryglf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfojvtol.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtavkwrv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qklztwea.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hitiuhth.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mljcgjxh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rbduslwy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3velzslkh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3sbqztczi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eixqobfd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3etrlhdct.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3grevqznh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gqcrysds.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mymijkec.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ijhksuli.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mxyzpfro.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dykhmniv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hixikgqz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yerhutpf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bnmywflg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ukxthosb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gzfddhkn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tjtivyup.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rolzozlg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzwccoxn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezrvakmg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3tcgkzbdd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgxxzvza.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cjbgbjbf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3expdbvdv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wynoexds.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3npbdyhii.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfhtjilg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3siggryiw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3llzymwmt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xsdcxbno.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dmjppuck.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3slmmtpny.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rqzdkkbu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mjukswzc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3cxypprsd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3obaoukhb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yotkifjs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3drdujkuv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypevakpf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbjbcwfa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmwgeqab.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3efjpvwnm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3olawrpgc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tygsfmlt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3attfnjyu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3opwcibyv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cgbbvyfn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mvukcdfo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3coxuukve.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fypqcwxd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fzvylxme.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3auszpslx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wioqukal.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3peynnnuz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fnqabngt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xagqeltg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3krkemdoh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjbomjdi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gfwiwlgi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pbnlhamn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3pkwirthv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nqsnlqoj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gjaahahc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dktdwdlo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ejjquviy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jclrbarj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lfmdobwh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ikmetykh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wkitveot.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xrffmdqo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lrjfrbld.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zkcrxpsd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3npeackbo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kkcuoujp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hoauepxv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eagibpnd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jymaqnrd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jbvlcnye.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3spztaxti.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bqinyxcx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tzcmevrz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gahdnhcb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qprbkkdk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ppprpuog.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iasdftwh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbqizzfq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mthhibvh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qstitjyh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcuuroic.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eglpiqzt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3uhrsnupe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rzfvqvfb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3urazcxyy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3epzwcqop.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fydoalxz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rrnaoppl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ajbqwczd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kxrvaahj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vfoalwnv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lcqvjxcq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xoyxiktu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzrejoyj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ixrisnxa.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dtozzfht.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kzwyogah.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lgjvmmkj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ldvswevj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bcokukik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irgwadim.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sjypigbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axzyfblh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zmjtdsyy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cgnggjnh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iphkriqx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnqrikiw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wcoyqaws.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysuoituq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ukljhhvw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3doizdjfv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qphzdytz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kekheaqx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3iqsqqulc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hswenpcz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ivlcirhn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jjrpiyln.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3uojbwzrz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xdsfljfs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yzifzeja.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3liummamt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3yshkttmv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pphemrna.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnzbtntq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uakvdzbn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3iybhwzlb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hbjstvub.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3difvmtgy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dgqxvlag.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sywzsaza.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3fminrgtn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qnyanfio.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xydoxupx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aattdgak.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fudiliio.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3evbmbprs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tpuxzfkb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdmuuqc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ontuwcov.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3invhvjle.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3utekbfon.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yhbvcucf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yzhixykq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xtkmnnqa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bxhezjcw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jxysjozc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qrtsgtbk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tftqlvte.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xqfilvbn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pbcfpsew.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3chfdiorw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hbzrgznd.html


<!-- 参考信息 -->