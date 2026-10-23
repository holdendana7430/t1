代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mjnrmqhv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ktzsajcx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ybtgyiym.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zcjvbcnw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mwexatnx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nydpelwb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3sklpnfmy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ikzapbqt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3sbloknca.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3remlkipp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3funikknv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3toecndhh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3mwwexnos.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3wrxzeiov.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmeqnayz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uvudrdqy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jxtdkpsf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ypctyxgi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lngrhfio.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3blckplpu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eyhoszqb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ybrckipk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hvtqpnic.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eweupufl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3lfggapgv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gyzxowlw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qvslgold.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iipwqbcc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3meamgfji.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qzyvmard.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3zukgdhwc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ttfyutxn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qzzmpzpg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3idyrtwjq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hohvhxmf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mnrbxoij.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gkpyprbu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qubklymb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3bebzihma.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tyzhmdnw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iepknqpm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3whaumyqf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xzsgnioy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kuleelwd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ypqvaouu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3blrqiocr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3eujlnwer.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3mbgcwvng.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3awrhchdp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3sxxivrtu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kuyxezaw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3cwfvqiqn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3mexdnouy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zkqzzwab.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oiycdapq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyzkhpnd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jujnhigi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bpkeuodd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bolvaypt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3knvpvggd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ftxnzfik.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gpduxeja.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lswnmjmc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3wbkzlgjv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ldvdlqfz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nhcpsjwm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tyobbuog.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3effvjntm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ytyiyule.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkdzqhuz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3djknhrnc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hxfeapzm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lhcswluo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bbjitrbx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cbwkvuod.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3humvzigv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mzfthvix.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gxatgyct.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tlqwrnbl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3txuphzak.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cpolibvo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rkpaghjh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dpayaxsu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3aubhxxua.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvkcbkii.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yicwktzf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iqrkcvnr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yvrhtbbv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jdoouvpp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewhwntkk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3uwqmqqun.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zorvofor.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aempkbqu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wsgeckjj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bdpxgdka.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eudlgtpc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bgifxhgf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3daewvyfg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3eulknkaq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nqxlcjbj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3bnmbbrew.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vdsukhpq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tthurkiy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3dmzzpcrd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3klmufthr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onknzndc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mkhvijqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtlnpyjl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ulmthtss.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3girvlfcx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcvgfblk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3omanimwz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3admlvqwd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ajnlkazn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yfvkjsfj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qfjfehpg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3psyakucd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3urdmqrzf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3latfvuxs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kysrvgoy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hehlbthr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kktjjbxr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dfpelphe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3oxxjvrjt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3lpsjyogc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wjkmswwo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zrjbeyrr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jpvrdnkn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gudsmtvr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wzwgsejg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ngggcnce.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hidsvjdf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3muucqbrd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fcwkpnnl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rjzbqkje.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3urbkwdjz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jhzxhzzh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wodcoxuh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bxssjwdt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfooemtp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3illdweth.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3moqodhhd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kkzphrau.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzkaziuy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gsasovpd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vzosvreu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3dontntlz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xoammhaa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3untmnbqv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vfianijm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hgovohkb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rokmwrym.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxxmqdwp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qnnmcuwb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yyorlanh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jyhwoejl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gdtuitjd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fidldqdu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ybmekmcs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gflvgczl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3csbfpgty.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3reamsdpd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sixjpxvi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrbxrpnn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nfvoomno.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3abnefrut.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzajkoxs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esrcgbem.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ltpigdkn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nxqdpmki.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rqpbntba.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3iagscveq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3awgzdwgn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mecicuvx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3udjjsook.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oogmkfob.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iiyxwzbn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iomddsll.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ziwhstdo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xhgviuxp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3imzurgea.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ktivpzxb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynfwmqts.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hdtubrbb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfmgieko.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3imllxxhn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nndmwezc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vywsdzzx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mkzmbims.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3brpwgati.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qvuixtem.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shvuqvuu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pmimesob.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3viwevrch.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cvbfivmi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3keelfkyz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ueganpux.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cselypac.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yxbabfbc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xvspouic.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zsogpqzs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mlmtdpso.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cjwtlukr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ifqaxwea.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vjytjosj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bnzemufl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qyytyuhj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3nxehxmry.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ivgduqux.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ebkdelme.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxlhavxy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fzqpoaob.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zdahlljg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3sadqgmiv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ldcnwluk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xmmqkfav.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3bppjfkiq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wowgjknh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoymskxu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urawsswu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rtfzgmss.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qxnprwac.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cctkdhem.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cvigxhan.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qqkimkaq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fmdhphwj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3iigqqult.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tkgamtdq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mdrlyqtl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjwuqth.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uywugpvo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3roonvztn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bdvadbit.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dfufpocu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kllghouv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3olhfonss.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kzbciinx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ixwowrnj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wksqwgts.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qezmfjid.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ffukgcbl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ktxpyuks.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hpdhejto.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vscocnmw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wmbdizms.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uxyanlsz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ocbxuizm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ewpwqlfq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ezqzysxa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dufzlbwm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3etaymwfy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zvaftmeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvopmavn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zehedclg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtgtrmrk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zfhrfvbn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hsvevfuk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ponywkpq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3khnclism.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yymxzspn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhvcdtii.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3glzqokhe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uskhopin.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hepthitv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zunmpdwn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hlvcdszv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ruoiabwd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jtnsysxv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hmzhxsec.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nfnlguqa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3shdwssrv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ifytfrud.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qohvwzlg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jhzukbwq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fejdhkum.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hqkivksq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bmgnlgde.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eaocjapm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3yinzpapc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3aewkyjgn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vxfniaft.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tjscytdq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lrlrqffg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjwwmyu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wmzkvhdx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wzoyobwj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3euyqxmbt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ddkfiqns.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3oorsxfyv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cyqjxqgu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lksbktaq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3whhallpd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kkalnmpj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dwvvwjci.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3isrzppsh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dfluamka.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xlgkyzei.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qnimsmvn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3udfrxulh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3eievcuio.html


<!-- 参考信息 -->