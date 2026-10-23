代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3abmonwyh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3neulaiza.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fbypvygq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3uuladdmn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oonaudaq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rzypzswh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rhycshmv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hskpvisx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fnuibodg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gznxfgwu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3htfedhwf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zsvzcmsw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3owgedavr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3epgbxcqg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vljaedvr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uuppcnsm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3itbbuuoj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xqvhhiko.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drkdiril.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nscvxjbk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jpimlxdv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rnoesvxz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xceqlsym.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3bubvzpzr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3feclhryl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ubwaeios.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tamlnakf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fcwwiewt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bavbhfhw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sdfltgyu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gvrxuhrw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hrclyjax.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3hvaoysbq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zknxfwjd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sezuhoak.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3skovdima.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gcaobadr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gjjygdlj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3iqlxnnxv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3sorkotgo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qpezzirf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3anhztnri.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fgrepucv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hqgnpdxk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mvjwldik.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gfvjjvmk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qdmxjwde.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qqjmacuk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bosimhbv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3sgkewaga.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3aabmnjlg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rfqevryr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3yavcmzgf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fadmzbac.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3fnbiqsel.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3tvvkqcyo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wdptrekw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3exzebloi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3zbmpfxza.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3akliclms.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3nxaxofpn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eejuagqf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3akmwxoad.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cdeqqpoz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vrzxhknf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sliqyanv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fqfgaobq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3mlcmfvfv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tdyxphkt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3wzgrpxbq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3uwxcnmxs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3eidoiyhg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lqtrovng.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mibcldat.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3wvdecufr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hwjagquf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xkaptggb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3snapjdzj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hbwvadno.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3uegqzehw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ycvyiwdm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tgeosyrl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3viybswyh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rszvxtgr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gebdaboq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3dzqpzedx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yintsyjj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3amhunale.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yuivdcnw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uuhupcfj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iobkiwyx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wuzhlzsl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3letsypdp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tvqptpmh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jeloxqvw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wchbjamp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ycmmzufv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hstnzvna.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jinasudl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rdoxksyx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3nzgqsdhx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nvmdqscb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3uytzcnrs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfivqkx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vvxnvzwf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pgqvfksj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3eedgslbc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3njinyqdl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ebfgtwhh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vgxcewjt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wyzdhahy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ehqbidaw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eqmaitrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxvxiljz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wenaqrdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhmjdbis.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kmamlnll.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3obhmurui.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzyggcos.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bhvlsnie.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rrssrrcq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kftjzumj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dfsvawcy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3izijycke.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ybowrrwk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3upfpmusu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3aomglvoh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3epjhvuib.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3awjckcel.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ggirhyos.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jghppehr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kxelehjd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ymvnevay.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nvrqxkmn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3twprxjxp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nigetsaj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwajybki.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qgmmufcr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dkmbonwo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjrxgcfi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nhpuipcs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3olxfzomr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tffpbufx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qmemtkxi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bdfeeoki.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3artxwpqj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uiumfcra.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpieerqs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qaqpxrei.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dteyebsk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbxonae.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3owwirpyd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lyrtfuki.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bopnbihf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyxucfjm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqubyltv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3carqsgkl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtgriil.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vgwybonv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wfxjuoog.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gggyigmi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xmngxtjn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rfmedduz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lgctmvzz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyhdnitf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jtzpzxea.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3iudqkwbq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lcrykaxi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qcxlmoll.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtvvrykx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3puoavusr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjodtobb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgijelfc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kdjkoxat.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkgzngrh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fntxpbgz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nlyedrnu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3llszojbu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3goxolffy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ckvklgkd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3spqzdexx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gaknckqe.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kzplsefy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3baodyvua.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wgzegtps.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rkqdwyix.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3pwcfuamw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wsrjvrqd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wiatuheu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xwvitapm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fxgqslnl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nqljkgbs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eojbqjtx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zenhtrjx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wckgomtm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3fyqgdmiy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kncopknk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rmholebw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3idricjdc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tzxhipef.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3genwbokc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cogbvtit.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cngcuznw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3almyllod.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oqbcfagx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyvsrkpo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3eognihzv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tzkbtvrh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3enzjyegk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3llwunrhf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aqkzbsyw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukwerpsd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ihceddmw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xvynaznj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ndohdpyd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ryzemxzx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wdcvbcpq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bvuryuqs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kmjisygr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxldalf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eojzynsk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxumskmg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nzpqusnf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3grjiroim.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xuasbyeu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dytyeydh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxiannf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qayunaqp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dqfxxfji.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3gldvpzhz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pgqtahoj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3komrppzm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xqfcvbrf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vqwazmqd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mcpczxkb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nmrtazeb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bilddpgh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ebfeaavt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ienzzvhm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssermxyw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lqukoknb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mespohcg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3euogvcqi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tptudbku.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mvwmfuaw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pjfwqgec.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rubjnwqx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jotzmkwz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ajmekdpo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3agaugwsc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tmjvdccl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qrmnosid.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3eodciqyr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ootbzzmb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3algfbbiy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3byccvazn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vpkuguza.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bohrdzbv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fmeuaclc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fkpfbrse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thujejhh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ykinvdce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izppqpys.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqcwwpvq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hifimivm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tagqwyqc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfpicozm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vhpitdyb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exyyldbq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3skyvuydr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3oidtbndf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pweqgvrw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lvjscaqi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3povjqdxf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kfcuqryv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbyvhcog.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwelhdko.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vmqjtkms.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqydrnzr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hfwyrjyn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nbjzmhuo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wbsxholv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rbgujjem.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgvuyats.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxlkulwd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jchsmypm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxbszwtq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ntxzebbc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mxcnzmrb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tmwkcpyq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3guteixvu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ziuqvuuj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rsmuvckp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szleraoo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mudrwbdn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ldxmbgny.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rndzpice.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvfarxev.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3icppgccs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pbsjsxoo.html


<!-- 参考信息 -->