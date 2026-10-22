代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2fklfzgdy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nbzohbhq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bmewxxtq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2isocnteg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2avecmqvf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2axloeapr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zqzoenjm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ddzvybnq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jcvqgvlp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2movyibsi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mzennfuy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cblobuvm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fkgnaubi.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rrfwqtzu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jvpertfo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2jstljisi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zguqsxsx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wosgrbru.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2pbfxdvec.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2honirldt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2edrutgnq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2zpibtkxw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzbygbkf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzaxqowp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2makchxpl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2oydqlsmg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqoyxdst.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hwlszkfn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fwwtdetw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rkchaypd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmusciug.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ehfowtzd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ioldewrw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hqrttyws.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ltarqgph.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rwnwahsk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2yyvoorgz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hietkdkj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kihoxyjn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fsdafhsx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jhszewlz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wfythjda.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wypfgpgf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2imaitjvp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ydxwtmls.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ievuobqc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nvyuevyp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2goanktzk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pejawwvm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dllxvusx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ioxffkmt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vjmigtdy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bqmlisoh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ilwfpaqj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2wpnokyoa.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ojnizpbn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2eferpvrn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hrzoaphe.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hoyxsrjv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2axifldbz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzpcuag.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fwmloahe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2jgebprjc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hhawelzc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfhhmkts.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdrjrbc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqgpfjd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbnerii.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dtthgwoa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rqaybooq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xxegravz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gssjndzy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mnrlkmhn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zbtqshvb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jjtidxnp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pamndnfo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dkjsawpp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yijidtkr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drjniwpx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nownrdhe.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2aqpjjuqs.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fuxbzahc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2yviqymgv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2eplacref.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2luabeulf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uriqivxr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hinyuwgy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2kbgzsmxz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mlkiltsq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2okfaglue.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lklrhtsr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nnyaghjm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hlxcfdmc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qweomxxf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ykoogesp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wjeewcba.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqbzovfx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2khbrwwvs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tnohcjzj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uttwkdta.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hnxdnsnx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqfqpmgn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfcqmuiy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcstfoik.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xvrojvln.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2swavmkyl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qjfjjykg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ijmzgtft.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zyzrjmnc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2dtlgfkdg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vlyrykpz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rffxxtwu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2tsiaelqq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nmsdfkwb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hggfxcql.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2boeyihwi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhwdyto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gncdqykm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2aqgsbcqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbbwelgi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bjtpusxf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gebrmxxd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ijfdjmni.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wapxzqvz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ydxkyzev.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wkqqmtim.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kwqasmvo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jbudcgma.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nscviqaw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lgsahgru.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zdabtpwj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zsvnwhbz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2daxvwhxf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aowbnflr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cpvpyogs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xbdmnrvm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2svsjcbiy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wyysnbxp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2knteqrsx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mxakeorp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jystlwky.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkrncfas.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtgrdkuq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2azenmhio.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ngiiujxx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dvytyphd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xdmysans.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rkmgooky.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fzuwvuzi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2rehuwxnw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2maakopvd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2amsebqch.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2deukwksa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2hrqyeeer.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2teochmoe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2axqnnogb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bimqlywu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ccqmokjc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ixwrtgnn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2epbcgmtr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jaycvndf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2wuhiprca.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vlqdaqpy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rifiyrad.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfcjbhgq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2neoeunyh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jyoexsyw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2iljkelfc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aciozzid.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dgorwdpy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ofxfrnou.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2bzpjbige.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2veeukadc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2plizwlhu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jvmnjlax.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ucdljycj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhhtpsxf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2foodpwch.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qudbruun.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2trsqqnzq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fgqydyhe.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2lqligihi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ymfkonby.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ucahfrwc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pjyykyrj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hazqtrzt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bkfgoldj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dnwlmrur.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qpdjxvlh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ieoeixxu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gxtvwvjm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yfnazdky.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dcdyvymw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2udxdxdtu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fstkqetd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzydtxff.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ylchwvuy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jtuumsoa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2favqpczi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wosrqtgc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqwdzkic.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ansowkis.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2urrkfjfc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxeksdpt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2asbpuhow.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2awoiomjn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2udeajyqc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qtosqqyc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bylkzsct.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2phkguczp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hquvvdip.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2newxhvda.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zpodboin.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2guzmcpka.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gvwdswth.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwiysnbf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2invxjopz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yactwfck.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhlgiwck.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2iimlgonx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ddxtzuuc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kjrfqpxi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lycxejfs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2skkeddzq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mmyduxjg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2aolrzeyh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vvlsswmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qkywemhj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wjxnalrx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bopuwvnp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jbvkmgpi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyugvdui.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxicwkxe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fkvxcpjn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2izzfgpdt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jnxqyogg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2sxthuqvr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2aupnpjyg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hfzbvqkc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nbxhihhq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ospcfymv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vpmykzvb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owyifvqx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxionaov.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2acxljkgd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obvufwgg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qebfwoje.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qekxaegs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wjvdsfda.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2psosbfzf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2flthyayh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fnmsyffk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ibgpzzgw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohioqner.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qzjresok.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dazvxsgs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dffyinyb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiogiqxp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vyvkfeka.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2scxsaqev.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2thnovmha.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yghxnfql.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bosefsfc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xcffgsya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izhyonhe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kyvevljn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svdghwre.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sixiapgk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nslzwvze.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zwasmepj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyeyaraq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mmudsazh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lgkajwej.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fmszahew.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2okcoqord.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bpwmncfr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vaabtihs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2psqxaagx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qusagxng.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ksifokva.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkjfbfhy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rjgrcyae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2fvtvxpfy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2msgnqeee.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qvcyobir.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ocslfzuv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xjdpabmn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xetceyfq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2msaftvrh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2urlvchwa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xkkklogt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jlisfpdi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rilnneho.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2eiyhrncu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pqsjrghc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rzoxcpln.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2eouyyffr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awpmnoku.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kgrsckhh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2txizpoyo.html


<!-- 参考信息 -->