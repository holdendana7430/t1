代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qyrczfan.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wsxxdjmz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qgkhpsgn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jeeymwpa.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mxihmeup.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dzezmcbe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gkaavter.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3frffwbuq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uzxdxlyi.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vxymhflr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yjbobiqf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ydudxmrs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rpkashzw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ibimtonc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxhbvnfv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hqtltbub.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3txklbxvo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pjgznrli.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmedcvsm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ysecytrc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vwemawsu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yhnjkydr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pcbnrmhw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iqtlggtp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmeonqgn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3snbpsgsi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zitplhpx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3msqnxajy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xeswfjzg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rqufmmoq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cwvbjoms.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zvfplzpj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lgoksvfj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qljdrqhn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wbxrsrsm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bgqnxgdu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3rveekfre.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3sjxpevav.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3arjvrvrq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3bciojeqt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mxihjquc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lubbawbd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3fjrsdoki.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3amnkwxrr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pbjxxknh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vaqftaor.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rtkusvob.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xatzmziw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rxjgrazc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kpvnppfe.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kkhxysiw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3dskkgxra.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3giyvyjco.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ygxczpgp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rrpdqren.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bqvvswij.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3lvgtryuu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dunkuakl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wtvbpfxb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3veauqwmb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rapgbdtz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fopmfnrc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hfrzivnm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnegztx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ugbrzqhc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwckerp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xmnhebhq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vbfavvth.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cfyeujza.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3sdsklkxh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gxuicvsf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3exzzokpd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zfbuxvnf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dkzdzpvi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ocgnjrrf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnezytlb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rcppnaon.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aunuksex.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kzwhbgtu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3hqvbcpmg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3svjpqzvx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zbhdxeec.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jnqiwyvq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wengxida.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzlhytlx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bbhkjeyw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ptmcvbai.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tizrwkts.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jaymsjgc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vfxqxcdo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ypjnwtsz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kvpayvkg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3bahgdhsw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vcpwxoap.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3awcibnms.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqduvzor.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3irkjovsv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxoxzjre.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ahpdwlbh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3aycabqvn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xyqaaser.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3uhjkhqrq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3nhepbnwd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ebxiinhq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rvvngagw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvsvelm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3beufhgmc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rxixacou.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bpyjfprr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtolnhry.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nshwrape.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbaskzio.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nogvewoj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ntaiyfvf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfuanvxy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3inrblpvl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uonedunb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eatnacpv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3esfeoame.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ytwxkvcf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dipcklwv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dbhcifwn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uimiplgi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3prbvgswz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3apkyrztv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aiwnbemr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fdmhhtwv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ozkkifar.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jwsoshgv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xgbykvhh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kvzoprdk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zpfglldc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bexajbnr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ckrirfew.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlgytqbe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3skophous.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dqoatohp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rszvyzuq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ftvryiiq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cqsqobui.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wkrwbuzw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuurkmee.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgefsuce.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nswzhhvy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dzwqprno.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dpleucyv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3omsvxfsg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3brokwxix.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jnffnvhn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pnganwgz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tzuknwrp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kvgridzd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3culmmkzi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3txalenjp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ueacahpa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zayqupdw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cohgjmqp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3svseppjp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lwdavyqv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lzxgodao.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rawlhssl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jdsihmkd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3rcbbvgnz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rrswfzng.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mnpviuxh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3oswgitta.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3beuaujhy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xoiwnbqz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfcohhwf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mydcxoaa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksyhfhoc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aicydhgj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pbawsdve.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tdxspptm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3afgjxaot.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3avdokbyo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hpdqvorp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sxtavyoz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xwfhbkna.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qhhtjcfl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rnivihvp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hzbrjaqh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yqsfsiuf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pkvattwl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jvhdrlxl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pclryoav.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mllhrrkq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mptlsxax.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgniituj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctqpsimb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fsiwwfwo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tqpgfxtv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fgyvoaon.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ulmlivmw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vhtiymzo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kurnpxsa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3chteckud.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mxowerdd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmrsznzk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mlbfsigq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwrafni.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lfxmlkwh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ijpbskbc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dgvduzxu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjrvfnim.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sxbhlply.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tbpsvfhw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bclamgpl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3upitdjhb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3frjgvorh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ctmonido.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ibctjyga.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mncarnwf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3omrwpkya.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oxctfxdn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gneosbea.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tyzonopy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztizlvaf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3aewzqwfe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3azaobmrb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ugqreynk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3bkfptwpq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibcmhqdl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qaxdwdzy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulugjigx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wtduyhxy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3onrjyfwm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gatganee.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fkuckyzb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zgzyyent.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dhttdzgo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tpmeaksw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyelmore.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hbqagypj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zbvyshcp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ffnqaaxn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjrtvnny.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgrbgfe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rueuugid.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3aqizmlop.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qyecnzch.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eqjkcoqv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cbzloegw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qulxbyxm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3okufhfth.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fpephqew.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uycngpdr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3unnbqdkr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uqckgvad.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3otfgvokr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3prrtczom.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ieepdlor.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3piydrdyk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wvjdieun.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tloazbkh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3drxfrreg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzgvjfzh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yknfazbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxgtuzjg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yypsqobg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xauuxsuv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jmmjgfqo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ouggsrez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmopdifk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hpecuruo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ioqpsqcn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ydizevnh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3srexhakv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3utlessaj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3thziwegx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3czukdvnn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbniegnc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xbygunpi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3gmagcfnq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqkeesio.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3koagmzix.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nrdsbpzm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3spurvbwn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3egpdtcxi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzsgbcpo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3shrnabjg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ruzeejsy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3idgwulom.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qiiynquc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lhehnxmu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zlwmldfp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dieyqjiu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mrgxhrsw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3iutiseox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpguulbg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3esqzogmp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3eeuvexsk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jqhxqrbh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mlzbtnzh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwhennip.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ktrymlqk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3btecajpj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mvbwrpee.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nbwgcirc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uimnmubu.html


<!-- 参考信息 -->