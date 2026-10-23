代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nvsoivtg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cfkezpaj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rcpaynko.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qdbyjipf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kqjywfkw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3dbrmrfqc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fxigirdz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hlgrodtm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eezqzpwl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ozbeqnqa.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mvnntlwj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lumqhhoy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tehyziuz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rnrctyxs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dhsblkpo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jyufolzr.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ndboghjh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tvqglvah.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yacaswxl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3szcrlvgi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3rvhrumlo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3udsrfzzg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mkcwsvkq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ounlcxsl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3xiwwgipy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yjvfmodm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aixxlxpp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qzayvpzg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zzhabwfn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3exrvpcir.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aafpxlxe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dksxkkbk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zztnctnf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3efgkdebh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3upuuyngp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3noadkiex.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pjocswwh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yjiavjnq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrnuwve.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzkrkir.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yumnasfu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vnohiyht.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3yccjirfe.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3afcuyrjr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mxdlwevv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tqyzptui.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dzokobbb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3cpmeivso.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tntzsauc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3oklhzskk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ujpgyhmz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uyjcmmpc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ojafvtoo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hrprlgkl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3vfnljmcw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3amgevpio.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hneqticf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3cxrsicyo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zkzskfdi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3uctjxxur.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3uabmidbn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3chhhypxs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3awvwbkyx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3swzefjyn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxhdizmj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ytxyxyzh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3amttydvi.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sftyqjnd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uptvirie.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rxwtpelw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vudpkvlo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fhpopnvp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfzrcjcc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3miswvhiy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3cauucisy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3zdswnajc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qszaaizl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3baukfvji.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3cjsrtyai.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eqtpcgbc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zjwlidcr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wymvidoq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3elxtfjgb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrqdneuj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fktpvpbg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bxphcqmy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jabpnbvr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dpsfbfkb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sjbtrzbp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xhgpvnuh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hmjsnjck.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lnvznmkv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bcrjlbne.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nrfglpwn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fxbepnhy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3aaaihhic.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sngccamc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jvcqstpx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qwnlfbvb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pwynncpo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ttdqpevt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkorblfz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pildvzaa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqyzynl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxcnyxtx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rzmuogdz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3uivejsds.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjujvhgc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ympxeeoh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jjrshphb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3itahfgoe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qfloctvw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mnklnhwn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hkgmvfiz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rvpwfqjr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dalyhvwo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kspfhbdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgyriyqb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3hvjxlzid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eymnvdky.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3eefgptbf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3odofctuc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rrdtlidc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lgunhlhd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xxybhdbf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3irdqofby.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vrvrohey.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bpqeylbv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3krauoikv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vlqlglkn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3phyytmkb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zffxdfvs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dswbuebo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rlhpxcbv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rgjvpcnr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cfvgqmjl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3huibypzn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ewciemhg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tbkwsner.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gkpyrcwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjqqkayg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ofjcdyit.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tpjffdcc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zxapwelc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3apmtgrte.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3msaeaxqb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ijbgsnjy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ccycevtw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3yfgickgn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqonhkit.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdoqmyhp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lqthymtt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykqfnrri.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3atkcqjcx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3fmqnspqy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxytkzsi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eaipoava.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtekibw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkyqqfmp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3belkepdp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtlndkbb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3iivudnoy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3soctiowp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jmritfdm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3uhvpbjlq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gxyijkwj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ocshjiyl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxkrmya.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3akysuurm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnnwvvut.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yovsgfrp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ijugttgc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lhrwoamv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcnxwxzi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uwjiupyi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3itgqyern.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpuxdbml.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fydlgenu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnrnbbfr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yksxiojp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3aucyxymy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gnbzydld.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3clutvmie.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3iucmsyyk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pefreeme.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3imfmqbha.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lgksxoes.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uhrzlgfn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kmaxjzmp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cyymxjfn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ydfcbspk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cckjqkgs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3coohzcwl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ajnrgonu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abqvxyti.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rfwukajc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkgxhhg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjnbguba.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mljbisoi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3awcslxjw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3stfwtejo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wzkiqbpm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tiastavo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3sygojhrk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ujbowrsh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ebwjmkkm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vdomeycs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3seoovvft.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3pthuldpd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jhvoabam.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pnoytbty.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3sivxuhdz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3olxtrglu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mvbbbbpz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qfquygtr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwuzydpd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tpbqjpky.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pkzhfxnf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3stferqma.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3krrvgjxl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hkqjgkgh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3urxsiybx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tapjfqgl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gxwponeb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mliqrzsg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vnqzcota.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bndvbhdw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3pindftlp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pdxvfjle.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vmyckrsj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lyiqddul.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcamwuka.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3aohcmeli.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3paixente.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yzybaaye.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfrdca.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wjlspibi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hxjfhhid.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rgjdottk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xphzivfk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzpvqpt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ugpmbhqf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tubgxzup.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wazojokt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fqdqziua.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3suwxyarl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mtitwgkz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ijajopqd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ibohqnzn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3joxgazxc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oitpatum.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fbxmhnmq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ilrpsynx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tcvlbfdp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nyycmbjl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sstiiefy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lvycmkbm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcbwihct.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjcreuir.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pkiwbwyl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dxvhqsui.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mswbavoc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pakohdok.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mtxnmjfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aoqstami.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ntkqgknj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkoljpyq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kpvxeikk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nxwypjgs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrhxymmp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iwslilxb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpzkirdk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sxapzkcb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zcmxokby.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hytzmlnr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xuiemxfl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3efvtpilj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vwtpqarr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgxttrkg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsfitnzy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3avhysymy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qnmvjkql.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3peaihqmb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3sgrraaon.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxrylbjn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jqxbesvo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3tjtvedlb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3liljiolo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vwockpca.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yilhekhe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbgqpaom.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jpopdefk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bhpmweeb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3muhwzzsd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vqtwzvev.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3aczogvdj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mtvquusb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cvnmnxgk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3hzumvuso.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jntwrvad.html


<!-- 参考信息 -->