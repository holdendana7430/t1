代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wzihylab.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3amptzyoq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rfoudbnj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qiqzlhsg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tqlffcyn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hrudzaxv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lqcfmhyc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jflrogxn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hudtweby.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cbufiqkh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3emizqvky.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3djssvdyb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3mdotqztk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3fenlznnd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqtbaekc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3fgycgrzs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nlcmulsj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ovavuopt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iebwoccg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hpvmuspp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xmqsloya.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnhzeabn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptxohkut.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fwkasulh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3maupeamu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3etgmpvdi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3clbkqycp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hnblgxgj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3znscvrfh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3isxbnblx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mtyjqjps.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kqrvibfw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zcovjcmp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qucegqla.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3afbxrion.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mgmciird.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3iykoxnqo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mfrqukjf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rzwjdrct.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bezsutwd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iqiggnsn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rbvrttft.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wlocncqz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3phjlxnxo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3juqqmzbi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3llkkwgui.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3jvehmcql.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zavycndv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xhhuaqkl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dugstwzm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iplylvqx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mbhhujfu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3uxcdltsg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hcmhaxih.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ofacnnys.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3enatlrnl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3iojunshx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qwmwhskr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kohgbflw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfffruiq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wvcbuisu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3czzcthab.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vbctgezh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ltsejzqd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wsxixqsi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3kakxykmo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ddbhesqn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tytuocbr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3sbcfutzi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jnaasrnn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dznclsyq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3soeqcyew.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3trcmecfu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3enupsbmr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3gtytdngu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwyqjpbo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3meprqnsz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3khldadhs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lakiuxuo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tnszgmxh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gtcdfsvn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ylmwnzia.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jmymrxdt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3fkcehdmj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3aemevlwa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mnmtbvwk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zojijbwf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3lvnhjbcf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdeuvpwt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ybubprhs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tytnspia.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jsuuawka.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ebjtgymg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3sxsdifch.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tilcgiya.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dbzbuxjk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdxxsrz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3czxlxyot.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yyqlcbsa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dqkykcby.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xjilsnmt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mhfxzxso.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3crcuvexc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3egymmajd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pkttceyv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uiekofhs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vnntqfzd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fpedijzd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3znpoyqjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvzssqzz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tphmfnpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkkocuuv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cxswetwu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mwsbmsdz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3aqbhskkd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3smtdefpx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vvlkrjiu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3duunouew.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fhbzzray.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xmmizgxx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3apjusylu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hsfadmty.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3adpmadjn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3skbrdtbj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fwpsoalz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3snlznjuj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pzczewum.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3giikhrrl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qtexnbrc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yswhimxl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gdjiztpp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3yfzdbruz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqclxylw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cuyacbsw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npmyshsm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yokmymal.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhlpeofs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3jwlxkxgv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nhyudjec.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sytjyipu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gfhvbhqb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvwaxqp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lujrkkeh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3srklnrwr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3uuudfrnv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gfpqfycw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dxegdcgo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3axwpdsjt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qrnustnn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrvoajd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgybruxb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyyiuwvq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3skowvusp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nvecfefg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxiqwli.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qamziuxu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xltcwznd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3oovgpkgg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3humgzhge.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jrddpqlh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3axvdujnm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zdyvofvb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvwsqtwi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wsfudmja.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nraelxyl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3smnsjusg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3mmoxipyi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rwmlsili.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3evstznan.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xwnnhiar.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3akabhxly.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfyxiaib.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3uyoznenh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3moocsrdi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gehcdskf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lxqxmyqg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3golvgaoj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mqdwdkjj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jfelymoc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sdbbdadv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yumssebh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qkcveebf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bmubfyss.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fyznyfmq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3crfqvjrm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3weppnbqo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dtgiomor.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sigokozq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3teatroxa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfmktmiz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vfzewmba.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmylihfr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3piuybnio.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jpvdoosb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3awhsvddl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbylyab.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jcbvnavk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jgjnqhiu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpubqgya.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sexuhwnf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dephuuaz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3juhnokxx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eqbhklvf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nsrkugfl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nfjxhiwh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kxfczrki.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rbttazec.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jymtrvsw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wwfilajb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kjuuzoje.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3evponstt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cuzkjyyf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tpjvnqvq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3etaanmpk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iirwcifo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rkryrjke.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rqcgccuo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3siqkunkw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lfuiikdc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nnopgjwg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vipbmtyw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hiyopygl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgalosze.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bfykaxog.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yyfklype.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dzseeayr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3brvczooe.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3axiqhavd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dzqzolun.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3aieermic.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3epzhmcsm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3coyefccq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqdqbubg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpihfaz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thocfhay.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jwocdztb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xxpkduli.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ucnwohjc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3powtbwis.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3edckgufs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nedsinbi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3prvrmbiz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3byslalit.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ubddwybo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ttegujmg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kenumctk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hwzoeyew.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rcwqckie.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xlhwktyo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3akozvmqt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hpuxabai.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dqpbkfvf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zczaealf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oxpinwam.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3efnvfhkk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ykemeqdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqllmuif.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ssmmgdsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzqgvkqf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gulwgdob.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cgrvmpvi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mraamzpy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ufbfnnoc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3swdzlvad.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3guaxdkxt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3htvrhwov.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3roxhfkfw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3effopvwd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ilpmmsbh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uzfpavtn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mddagvzn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmccviys.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ffvgyunj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3szsbhqpp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hanlosay.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hxnmulse.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3almjuubl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kwcrulmn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mwsqrgtf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3exgxflsz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxnhpmxq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3enijnnlg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vipkrhiw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ycttrrcf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cvlelvdm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cdqlabud.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3snovgwgs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vbjvpnqa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pdpdlbgf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eetndbxh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wskcfota.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dxhhwhmx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3azxbuwik.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sjxhqjti.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwzansig.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3viizchpp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ajpkyqbq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yghdtmvd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3brzinrqu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3twmckojl.html


<!-- 参考信息 -->