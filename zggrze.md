代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eltvcvqu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3fevoayjr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fyvkcvkx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3muvfywoo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uoyfcjxf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cjhfarfg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wbuymguw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3secophev.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kflqvuej.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pnjxyzua.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3drolbirf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3qxrghlyk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3awlvnhlh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rjvhcfxv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3nlgfdbhi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kijyohns.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3lexfupkx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3smuwwity.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3croyjnjw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpavufrc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3zrxtbqyf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zcaestoh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqgfnxoe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zlwizdmz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iecnwmav.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3keooxfqm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ywempyxr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwyitjex.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wwwdjvez.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lcfbshjg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xsowuyls.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dheffbto.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3zzjkqqzb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wmdcbocx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3raxsjlpw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3pfjhbqwd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqddljd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qmzcrzlu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3qsgvzrkb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dzoyzhzy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gvmnntba.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3elauxkio.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xhpfiept.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3lhnkteps.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xuzxzcee.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vikpsfoe.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fyzhznmx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xdjszbab.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xdwaruqt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hamqmywm.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xohwbppu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3yhjdlqks.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3udfkiejk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3cqvphmdc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wqhjgagb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qtokxqlk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3odlorhdo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3teyoxeem.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tsgcfgpo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xtcqaumk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzoxoysh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wcwnrvfr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdagjrar.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gnfqtrxv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ubsddhlk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ohetvgpq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ljufdpeo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3oyymgugm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xjhgspsx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3vdolosrq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ebabijda.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3krttwpvw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cdngejcj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uflijmfh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqybhfi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3heqtxlpj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xjgewzrx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cbfiwttw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3arnimsvc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xukrzvyo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tpgnjkxs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3elnnnjdv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3senpscjd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3bwitjekv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pfewutiw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3syqphuoi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vbyjpxqv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3srnztopx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgpnymh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sedtafdx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ijiscyhg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3utjtoyrn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xihluqba.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ogjouqog.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sujyrlsa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3simepybu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fesamidy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hrjzolem.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhagwunb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3faetbhxp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3csjkgqil.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdxlmzeo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3bajtgbez.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmritaq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jvgkqcov.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3efbecnep.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3xjdijfdp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fygojcjj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ruliwegf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tsdwbwhc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3fgpbbmcc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tbsyprno.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lwonkqbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrrpkbvc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lcafufaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwondnae.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xgkybrgd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3twqdgkfj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3aaueqhwt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3atlwhomz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yqgpfnol.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cqhfsjlr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dvxklpoy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dgwmrmcx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bvwsmbss.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zsaakybn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rykbhpkb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbsrhphb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xoglntfx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uzitvhzn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nzeuvpbd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hvngyqmk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jbdythpd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aehahhjs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3thnbnzpo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pzqkkbnb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivnhkaxh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hgrlnpho.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtxdfmv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phfnehhv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fuckuvlb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vfzkktxd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fnfrujzr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3icfnpzad.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3glcujrzx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ffyjqxyo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qxlyuopz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ofnqhmpo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouicguun.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jhabxeui.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zclxfesw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjsyqctu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3csdxsraz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3cptipqyw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3grllopue.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iqcgxrjx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ugztalpu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mldancud.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tmkabsul.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nwnqkfdd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwrauari.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cwullwlw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fpfapsep.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjgufbqo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mikrgnce.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxrkllfu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ftkcqmyh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3etsgbdfp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qsjwgzxc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aszvgdov.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rxaqbkjn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hsvjiaeb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bbdlmtew.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ewtluxbb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oelqsdjd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cwfgfyrn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ifraisyw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrcwsrtu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vvigtndn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gcnesmge.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gxtwjzxm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ixoinjvp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3skwrbuqo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uhrswyjk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wasmmsni.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bfnvfcrz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ojwljmih.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vremnrhb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lovzfeue.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3iueqvxfo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3shapukxe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbacxlpb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mjcuygyh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3axqttadp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uafiizlo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3evqrkzsg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gzcvuwgt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bofysnyo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3flomlazx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3diorclbh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wsabkcsm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iuufdmse.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3maobxhzm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vxetfcbg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3smmxghhl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3trtbgnfp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3efcphalg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qmbcmugm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kjiihgiz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lxixgedu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rqhqmpsd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fismplbe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fhobgyhe.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pqkidsov.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tqshxhnt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3iqahmmpz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fajhxgtf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vudjweql.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uamrrnnr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pprifgjc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gyncdxin.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehvlcqje.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3umshjeqb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ecwffnmq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3wdcbctod.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cycwmmis.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mhiuvvyu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lihbtzsg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iezjengv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ebuygjas.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lexffnjl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rlktnbog.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3utvjtvnq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ovtenqlc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pwedxcia.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3uelqmxym.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wdzxjdlh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hhnwfcsp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbxahrw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdcyfmyf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuiialld.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3difjhrvu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3dlwjkmuf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3crtyibth.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fbmbvfye.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fvbzhtjp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lmiovvct.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gndapmkm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qajdslwk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jpwbgoom.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itwvaybt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3btwxjewx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rkpuqqop.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ghggtpwl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3quymwqos.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jiuohnfx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lbxploea.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nsxerlgx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3djjhwllh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ugwymxdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oivtiisq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3sfyqebyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lascgqgt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rdxfehmc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kmsicpsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tttyozki.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hvbmhppf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihvzenml.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkyawjuz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3dmlhxhia.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3iwxmauna.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtzgpgke.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3znkhecvc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3igfqsocc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hutlkzte.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3revdjntj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jopbvecx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3oxwwdono.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kdvtsjiw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3umngvfje.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ryetlbqg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3aeqjqkbu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3totoomop.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cussepnm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ycdsvxkl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ecseijpo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwmubpn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ijplgjli.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxpuchmq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3eescannq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xvtqqdov.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wbfdvpkm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ganbwatw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gnsnluyx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jdezxfab.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zgxcqvuo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rebdmcpn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbyhgjot.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dqtrfrax.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pqiunpya.html


<!-- 参考信息 -->