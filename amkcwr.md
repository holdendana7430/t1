代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ejlzxdee.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dtcsoajj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3yfgphuwn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ueqvwtgu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jvwjmnij.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ovmmyerk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3unnrssxr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lxdkvqau.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3sgksnrnk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wdsdbjsu.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmxmuzcu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3btzuzndq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nyjhobzu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3uvpsiigc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cdarvuhd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3dhpwnuds.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dqcuzhxf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmsfanvi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xepnhwdp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3guzlzjrb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrdifrjw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3erazxwpv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dbsufrho.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wernrorz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3isqjufwf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qwksxnwm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nesivsjb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cvjvigcn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3phmelyvl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lvlbwyka.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3oiftncqw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pmseporr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3khyhozxy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3kpjuwgdv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ebbkmltz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rdyfzozw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wkxednuj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qwhjjwui.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3bhlswgvi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wafarcag.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gfipgdbn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ixyavbwj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wesfcgqj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3zlxuxulk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfheva.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cotxpjxg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3itrcyjjn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3igshydfn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mxokwuol.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3jytatmqe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3msiaprom.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3uybnwary.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vvdsywxc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xqezfdfy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3telcciaw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjiljvuw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3johjzyik.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nrapihrn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zftvtjjw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3oflynnkq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oczbxjnf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzrsrlw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dxldygjx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3bbpwzbpk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3svtsolae.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vowzgyet.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjipocpx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvhdlmif.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mtxddfdu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hqazehzh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3olwivpza.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hemoypri.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jrotbuxz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3utjuoefu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aebbtlux.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kdzdvzkd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jukyfkgd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3acrsmdzm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3upbtodmr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fzxcavgh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3swbjintn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rbdlzvur.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nzixrngm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nlxfucdq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nokhhkws.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fiohnued.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fjtxrkug.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tgkrnvly.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zzpspcen.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwoejuab.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lqxexnxe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xrmydroe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgixqgh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3klspwgqj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3wvfckopj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kaoirqko.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ptisjokd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3aigqeazb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3juazefrt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3znulmqlp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3jdqlzxzz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qlpxltoi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nnshsotn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3oyndytpn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dvclpbnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbmscszs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vvplmfsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypsjisfg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jekzkjrd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3idnquxfx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3dzkiybgq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cieuzahm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rhzwcqtd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3raxzlckg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3thaspuez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wyovyltf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ppbsbmkg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ajpnxjdb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lvlxqlxy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3reiqaabq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vzubhqcu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qdzuoaki.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3neruztjs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hondnslp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3lssziwji.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dflngcxg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yioogdbr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ivcbwiix.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxcokjug.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yflnywtg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcnwgtto.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eashjhkv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3frvixpjv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ywgynywc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ntmefejo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3joazazem.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ekrzxlel.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmlatyki.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jfuxathx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvabijfu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3czyyivpe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ujldkbcn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3iebiidhy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoatlnfx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gmkphnju.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hrawhrca.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzzetzfq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnpbwdin.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3datrxsje.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vizlsvaf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3afmkywms.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xksddcxk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzbqthcm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vnerwfmm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gszaiadt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbpyfraw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gqjqorvt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsifhxii.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qxdimltu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mxublddw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oleokhgh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3thojvdiz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pjvsdfpc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwfqppmg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyqczyfa.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdbkmecl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlfahquu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iwuimtkj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hekzxbth.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rkydkxsi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrfkoogr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cqayvmld.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vlvjzdqy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vpdkwzcg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nnfgalnk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3stcmxumy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zlbrjwyg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lnvfvagj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gvvmydst.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fvdygshd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zyhldkuk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3oxdduxhj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oddelybn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qosysotj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzvuvekm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xjokkjuh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdywsnq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kkqfezlt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vykfgxjo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pxsdsnvs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3pdhadzvm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayernvbl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ctsgpmvd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xwnmueoz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3viedthgf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kujcfbyk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rguhoakq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aognochd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gcrwoyse.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ifillmxz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nlkzbuky.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ddbrqnam.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ikubbrnp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pblupxnj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bgxzifcv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gahuwyfa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qsjolsgy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kptdcbjz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tfbkieny.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rxwyazkx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3agkmnfwz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tffixsao.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dmwyihzi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3knxeddjf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yimpqlmb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hfatqigx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sziogwyo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dmduufkd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbrxgqtz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3touicqfb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyrhdccj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kuvnxwye.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jpvqmvva.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3erycbfis.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3uklommwv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tgsimmkz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3exqessct.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3iaiaouku.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3inkpqrrv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xbkkzckt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlborxe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yusfdwmn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcptvxoo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sokmvmoy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3onmusxol.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mugvabny.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zdzsszxq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vwmyzpyf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pzvnuhkl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3trpjyyva.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eimezprw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3asfywkex.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vzofimza.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dhesgrbh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eqhmepjo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3orlenolc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bgtrydij.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mvmmweer.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3swuvbyzf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kdtlpbax.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3aajtpfyu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bjmhgtro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieguklxf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pdhifqwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rowdovug.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3orompvzm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xicfnwdn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfeilran.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pudwmnfd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smlcjkxn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fzctzngk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vafpjzci.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hbnqqjgc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtgyitml.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3pnhmccyx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ieeuujxp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3golxbebc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vybfvoyg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xmmrgoin.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3espapjql.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vobbvwfn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hsayarhi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rznyzjrj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktcyipgs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3amocukpc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3uwtajias.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxnrgeal.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgrqxdoq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ireujcho.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uoycrxfz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gfcyeupv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vlfqtllb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3oilwidow.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jjiejzby.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3yylidsqu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eqfuknlc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xwyhgkfe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bvbaiuds.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zxrqhrcq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gfmxxgen.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jqboauth.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xjrzieek.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3inafvocz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3etmibzzn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dmeyrqby.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vmqsbxrk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3adhrziim.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hbtrsvil.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lzjkrivt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zwtfjkpb.html


<!-- 参考信息 -->