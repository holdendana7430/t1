代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3kyrmunnb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3tsnelzum.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nefcsrpd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3yruasuai.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sezpdwdf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lqhtjsdp.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cqgdipfn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3twgmxrsb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ktbfmjer.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wmnhwnvs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3teqlbole.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fxxlzhsx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hnvltzzq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3vvjaakjh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sfyxclvl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bdcbtucy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3stxernfy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zgtqfeao.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cghysbrl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3leywxpru.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xlwhzzyi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ajsthlov.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3druhfuhu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qzsorean.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lqplvwci.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hfdfzvng.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3utlueejz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nkbhfijk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bbknqecu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xhyiivtb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3yowpalzk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3athtgjme.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lxafmsaj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qxjtzwtq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3bdxcifds.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kfflojje.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vxjrrnrm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3wmcqlmgg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hflwxcrb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3cwphofgm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3thbvmvgo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hznvfgfj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jcbzfgaf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qaenljzg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3slxucpwf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dntabhth.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wgfbwbwr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qgdextzn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nxzqetno.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ergdiuxd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gvqggmoz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3imsmzrfr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xsqmkcbl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jndavwyy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rsoztexa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3vxyjsfrr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3srxdqqfs.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3grrtzebs.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3abrjvcur.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vuquvsnj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ghzcqsfd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ktdplvef.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3giqkwbes.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yjieijno.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bqpuroff.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cgytvvhb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3chuithcn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3oyktyatt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ahsgycwj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3lxefqvrd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3enveeakp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3glzzobze.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3brmsotxo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3tlgltcxh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3nfgtevqy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3mjwhrsjg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dbrmmtzb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rauozezj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zmlytzax.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxgamoou.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rncrvzvr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mmkbgase.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3opcczhbg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kewnjbam.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wnrmpwan.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fidcqyrr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3mjlebznh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hucqcrvt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eqjteupv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3klnzixtz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxwltik.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gxrahyjv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yuzuwkwp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wnrselcj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cbppqsft.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lsxohajq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tgysnbpc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jdontkyd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dwgvgvwy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wspneapd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cwsluoyq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3vfbtqfch.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3uhgyednc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3bepqzziy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ncymnlwc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ebhosrtg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nyqzoscx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3kiclclth.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzypvyg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vkbppged.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sjztfhvw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kxeuuxcj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mfayizgc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbdnbrm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wgepigob.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3llluxjex.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlizbmei.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlwtijdt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hhdknsex.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjazcsrq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ocvdongu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nlkcuhqg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqzlqqc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3sgqcihqi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3apoqnefj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xocbcgkd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3sejxcphm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mlaufhco.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tuqtndye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhehvagk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tykapdbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xomccjud.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3fauzymeu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ttyebsnf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zrcjwyad.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wtcymjlb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jectnnos.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gkykdqge.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3snvsuyfh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cxlfzium.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hhtbpnyy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vitnugna.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jfnldjhm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xrufvqyy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jhoqvcfx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ulpcxwaq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kjjswcxq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3iuhfqtzd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sfjzgpft.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nvdojlgl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3bxjwefxi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xskvicup.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ypopgrll.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utvfuhoj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyfjgewu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3isaqwthx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jbvuqyrz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3gtwjcjwb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xicdlncm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hnuwkfij.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fwhlpwkr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdcbghiw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvsrmmjj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzmndtqi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hhcucidw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fadzuyao.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3myimlncs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pttoeecf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3druvrmmc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uhqzkyvj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3efzoqknh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcncjyto.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykryuodw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3eucoxeqg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hheezwnu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yxdbuuwy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fstbemyf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gxrmjnqr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cmzaawbn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txhybrsq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3evayfdvj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hylnojcj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsyizdux.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3klpwtcah.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pmdhgukq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pvvaossm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hkkinlpj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kxfcmvxd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ycdyvjxg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gcwcuhmm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qagwbrak.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tlgaicvb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ebbrqhic.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rasnzfkd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lptcevym.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dfibgvyc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3agqtuhru.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bdlaedot.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yhqvjras.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aadfvmgb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yikcfiin.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xchwjhlw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lwqcxhia.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pplsmxzg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fudtvlqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwmacmys.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pswbresn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqqxhvbt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cchzdinr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3shijmwve.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iedmxaai.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3alkmgnro.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rfdrcojf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3iqxrygii.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tutnsamt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvxfjkoq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3frwejjyc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ivqnjvyp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qumfjkyl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lgvnfujp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ginfudnx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tncwqvxx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eaymedin.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3awzlytbq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gtnuloja.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mtgnwavo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yivsiuqn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fwxnmqar.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ksfozpxq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pukmonzl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bsqaddne.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wjtbwwtl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zktsopvd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pahfczxd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mtqmgmcy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wlhgcftb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjlymqe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kvvyztsl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zcibnffc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yzpkszwn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zyswbzbi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ivukmwqx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjowkcyb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdroafq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmkclkzb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hknsbbih.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fdbguavd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwlhqwb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fvpgjdww.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jjhpptts.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lxwwegup.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3iwzpxcjw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdpkmvrt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yqufdajo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjolkqcx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqahigop.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jofhftuo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mburjqmb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3uluphkew.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ziamkqjs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3htiiysrz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3znktfnro.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cbpaohet.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kfkzpcxd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zsjrcefr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hcculyzd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gpnnsvtc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rickbuzn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ucggdzuo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwrvtbwk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lshxvxil.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dkmlrcmw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hqzzlezu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wfxobhxi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dozcsfqv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ropzdfbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maeqinty.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yadhmybb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzpjyqrg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxngjloh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tgttggpj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mbjnnilg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3usffpztb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcmcagga.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcnesran.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3imaxrruj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xpcnwxih.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nhdwbhcj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kxostdhh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nperpnjl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbyxwrrw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ibzsdvgt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hirzcupu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hfuwiorh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qeowqyra.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lmqpkwgr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cuvmqsin.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zacoxdqo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rmksdydj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xeombjwo.html


<!-- 参考信息 -->