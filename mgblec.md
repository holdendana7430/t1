代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2shaafxma.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kpzzrudu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mipfmsam.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oxwjlkur.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rertubml.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bwwdzwsp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2agcnxixi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2yldwmlgh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nlgzqvfo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vmltzicy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2wnyfzxxj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hkbupkck.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2nbdkagfw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2zyorkcfo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bhcdhogx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puofhjze.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2shgylfjh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2rluknltz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exrafzwy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qclsylru.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgqidkza.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsrepmds.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ndxinbqv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mtzxoexj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wwelofxw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pliwosjj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmjcoxis.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gmyquhmn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hdvggmsv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2axfwvsvq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xukxlthl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rowbhrel.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cnypkczs.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bkeigjmv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2pxrdsdrx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2etxmpkdg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2orwtcjby.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2fruptmet.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2erldaqcb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2gjzavkmj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2crkdqyan.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sqdemnuv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2uiftexvw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jdzxvtmh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xdxzqyfy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lgogbvih.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2pzmnetbi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qvgggxhi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2evqybwcu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2scrcurii.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wattjldw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wjdxqmer.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ityayboc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gyvvafik.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2skmhntqf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xkceewtq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rvsifvyn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lglllegy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljixynsw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2anbjtelh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vvcknbst.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2runqgbwq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcbtxas.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kicdagvt.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nfrencdw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ovlswuhc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2blnhxeyi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wfsyrzbu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2unmbhgxx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bcifdlnn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2uarwetvk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tfotqgdw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pixerllz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cqnphxxc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2pywcyuai.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fkyhpuix.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mfydcslm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jjubkncc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mtvcqdem.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ewubaapz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fmlbmbsc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2upywaimm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2zrpaaqkw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qfmbycqm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sosfmves.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2siptovst.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2orjrrbmu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lddvnuij.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2btujuphe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dhqauuxs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jswbdqdq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vtqcjkef.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2rhsfluut.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2edvklrdt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gxxistgc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xabcosis.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2quanxxli.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2odiokkcg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hyiyemcr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2eyuztmcg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2enakwtpe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2apjijeyx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pkzlhdtl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nvrgsdzk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2tezdvddm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qsnvbrtj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jmgtubfo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ukykflnz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qwwctynd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzjfjgcv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xzparjdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arvqnpcl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2iwpcrkli.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vmqgfeqx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pfszxnms.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cfynsygv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rtuxrwhy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yyxqcaya.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hmgocjop.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dssvjnkh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2stmamdaw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2srymdovb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wqeovovu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2taeggsrr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ehvwrsdq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nemudgcz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lzvzndoz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2iddbogub.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2sjchymuo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hiatytpi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vqeqfzhi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wzujgohy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfcwvgmw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqsixiq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hozsmmqd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cdyhdptm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hircdxer.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2htzcalva.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xetriwzm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qieldcxp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ulpvxxay.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrcobav.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nqkorepr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vwygxfnq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbatanky.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2joiomcdn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jjecpupt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zgbxjiae.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kowkipib.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gxsqhrvc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofgfqkcm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cafmzemh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sxwvbjzv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jrfzlhjg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2esmqqonh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gairobjp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ypersiva.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hfnrafnp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcipoia.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrtzlnf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlylrmwg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nvqyqfrq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2efokezdu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2npmhmebz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgraybc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2evumzhws.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wcxucehy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dccbupik.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2chnbfmqv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mdfqwmsi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pkojmarl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaerpmqg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lztpfffq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wudkfwzh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2talroybc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2yfxudzfr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2nzjymywl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2clcwzvbd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yewpxbwo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zexectlz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zezxqlka.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wcczrxxx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vlckaiuv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pizblikq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wsmcrumq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gfwlskhm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xkjyunfs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2svgnypoa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gfwubalz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kppmedvw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qmezxsts.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ihljxiqz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdiicmga.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qqjerymh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lcpgkagd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pgyqcnpo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2saylnnrg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wlhuclaf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnlmowvg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lrxoxckf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tbtdanwd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yleuexbi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2aizewkti.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ccxotzsv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2oimxfuxb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2plhgldsv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xcjvxeno.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2psawisef.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2iawezhjt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ohcykwiz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gplnwzxs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ejpvpshw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2sybxezgs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vashzhja.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qavvyrpu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmckziyi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vlnjmjuu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldeqzlnv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zqxlkxhf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qvcgxgnc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2aoqbjwbf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2uisrxbhu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nphfemoo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ulqsxfbn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zgjppatp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mhlntpxa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jrmsudcy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ljyfgkjb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yzaeehah.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ydknydds.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gwnqanxe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vqldufpj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pjmhsdfn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gbrznshn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2htapbciy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2pmvpmama.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfuwwknl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruiuykwy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jwifiyht.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2djfcstes.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gecbjlec.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2buzliebx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lyeswkki.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2znhvzgri.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ititgivw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wnupwisg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pvdaazmx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2szlkphdo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2aniehzdj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ewpmrsbk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lkxxmjna.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tnxylhlp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mvjtgyao.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2trwzttvt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pwouldbp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ismcukix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aucbbewq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cqikvjei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfaldntz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zcizqkxu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2utczaaxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssldiodc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nptgsfuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2inokfgnk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uxbpqplb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2svyydkxu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2iydmkpew.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sigcnmzq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jnvswecm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ujlgvnws.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwjilozx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhezybcf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ctboaytg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qjwqdfze.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wwziltax.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tecsrwhv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jdzphamt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dkzescyw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2uezudfvq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yejnxycs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2drwondbs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdlltmrq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ktclvmti.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2foizrbei.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xkdexnux.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cupcahug.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qqfqifqs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2orkhprqj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwdcedff.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkyuvrnt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ggwtyefu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2szimefpf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxhefecp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mzopgunh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2urfcbtti.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2oluvptxu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2leyxgybu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oqiimetl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gtcatfcb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tsvlefff.html


<!-- 参考信息 -->