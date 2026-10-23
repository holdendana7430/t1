代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3seuhkhal.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3joybkgkd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mkczdtck.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ugipuaao.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ideptfsc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xwzouztj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3jqndunva.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ywhkuyiv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lltsfdlq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fjfflafx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3jkzqujvy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bdgshbtv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3rrczobbi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3eueyeyko.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3fpgszuwh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrhbjeoh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3lpbfubum.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ruqfrmsp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcebsttk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3owopovob.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3obssqhid.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hjdawkpe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mbtyacgx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uylixfvk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kdzbnzow.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xuivltpf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uiwgdqvi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3medxknjp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mhofpznh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpbqoov.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3itbvetjg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fazhcequ.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tqseghfm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3cdggnhwk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3euhohfft.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jkyzexdm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jfhsmsid.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zltgkbcc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lszbrhze.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ilzcvwuk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ktfnhajr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3leixwbvk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xglydrrb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lvrmredy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tvlibedh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qslxwwrf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3eetwhlio.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3bxkjwako.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cfnlrvnp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kenpolww.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fqsfjazp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3sbgieavk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hyxjiimz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3sestqfnu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dxaghrdp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lztmqeud.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3snucbayg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3elirurjv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfbxeebs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhmeaiub.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uonrfmhr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3scwqjvsk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nbibnyxd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ahmehtrt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xmasybuq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfaolcd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ehibntsh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3fmefwtlm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sdpxytae.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3eeywucic.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jzyguniw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3clznaagq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uwnryulu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfiyeple.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xchxpfox.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bndncsmn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tglcuamd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ysmuvbgt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jdecqhsl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3aeywesmq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mlkncsmy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3husuopwl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zdvkactm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qcuvkwqm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3nebxdafc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nimdcqvb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3radusvpb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dbfzurxe.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cdjatxng.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yamsiitg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vckhkjyw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hqvuqvzw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3woiuaxty.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzdlhbc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qkrordft.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lvasbhvb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3jnqeetxu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yqwbjzah.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qipncnpo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pijyywbr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3kvpjijpg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3otvtagmz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rnraybgj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zydxeoix.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3avqujorh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kzavcitz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xsrpqobl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3noyfnqhz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vusclvsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqqpwojw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lxssvzlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dakolzlq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lzrckzfp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zhjiamyi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lsgngazt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pyuevfik.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qxmwzdom.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wbzmxusl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xwedorcj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pqwnibon.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ekebdkew.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hxgbzkqr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xrivzzas.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmohxcqu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mxkqjmdf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aotnwsaj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3usozcbvp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dknhcyjs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pwcxlxoi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pnmyjnhv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3cxenonci.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wmjecwqc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzcfewue.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmtojht.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cxelnmgs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mihowukp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bafszako.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xotpadlu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ixdllpac.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kumuruor.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3oyhpqzxc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dmiqvdxg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehijyjgg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ulgcpfkh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohmfgfxk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lksrkpqh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3vowhmnfv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bquvsjer.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3efvgtmel.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cqcyejyf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzgsvrc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3susyfbfl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ggambwom.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pjazozob.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zucvdjzr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3myttzhbk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3wytfxfba.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vszauuua.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fyibmhfz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ojdzvsbl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmklxpt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uztkchpy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3daiqtzvx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jwrwnmnv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fsqkcnie.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3idcuzzgx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tznegapt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3koljhenm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdngcrpu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3clubxspj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3addmmmpv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ikgghzod.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gignooit.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mafobzje.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxbuacri.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gyxjnxyg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3haqenrtm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uxagbuaw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gdjcmugd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cigvgkib.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qwwntwtn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xykwyngd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vdraammt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tmpdvoql.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lgervhpm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rugbejfh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vizpzoxi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpgxbond.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3btedzbkq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzolodiq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ohgtlugr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pqjoqhgj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dmxplqpc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3meldpybq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3erjfzvkk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhtvddkz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iwypsocx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3opuwpbyk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ftckkhfg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3puqkzpwy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tryzelqu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kptqpghq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3itrhqmiu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3gipyqidi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tcwjcgkm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ktgrfvfb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ijnwstrc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tieopmiu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3chljnjop.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3aealylqr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nymdsxur.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mgjipihv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xnvwbqft.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bniohrux.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lrbovuan.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cpljprgu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xmwlpjsa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dczbptzu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kqytdnan.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ibjqlwwe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xylidura.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3uyjhjbct.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3agkdtenb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yuebnbly.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3txovirnu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ppnhijmm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qoszmwrf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3khjkswpc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vtmbnvwy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jrcgqelv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xfpozbdp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3snwuzawn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rftfgwhu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3chxdmkmx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evdfamrx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zsnjbcmq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3anebkhfr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3noicaylk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lhtmbxdr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ypbzrcew.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3scfoacye.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wcnvwcub.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cjdbttgg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jpjaytrq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dolddbrj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hebszmpr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hyfcswie.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3txwlsfsm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ffbzfevp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojefpblh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gkfpouzg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sjcbsjge.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tmhxukva.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fwfdukna.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bpyogerx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3absvxsci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjzrqvqy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pzxpkvhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sauslrvf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nrbuphil.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wcyjjqux.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yrfjkzbj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3boagwuld.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rdhquyov.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rvhvdzvh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkqdlzeo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hlnyxqfr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3axttyssw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nyoyvjlf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vhnumjhz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rindgdel.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yvradmef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxzlinrw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rmofzpwe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qqejsbrg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ciicttoh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3toztabka.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sqlwrpzj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dqekjhrm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeglnbzq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cligajzg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfivbxli.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gvwxompo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qjqjsxto.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dovkcnye.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3aiujkqwz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hpbockuf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jbkmvvau.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jhedvodr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahsmfbzt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xztasmfg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uoeiyhjz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3oubotsyq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zogciajm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjsytyuj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xhsvgosy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vvwlsoke.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lafgulez.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hwmhacgw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eeenrkzr.html


<!-- 参考信息 -->