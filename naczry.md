代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rfbmkcqn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mjmxpfye.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bdcqffky.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2yiegnawx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hlgzoplv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2blzunzzr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fkkfwsce.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cspqjxvx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2umllvwfu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hzxopxkh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gpadmuld.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rsfhxvzc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nqoadbax.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kjexsgla.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2glblavzb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2wcshmfew.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2gfknuuyy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dlfcozfx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2vkktgney.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ggrojcos.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2baiawxnx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2choopibo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyisscoz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ceovxmro.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lggjjrhj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uiloeigh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kptysfio.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tftqvroo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nrzdupnl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2izjsucnq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sjpsrhoj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xmfgvknr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tmuyyiqh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dckquubs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vsbxqydq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqcrhhi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ztdolzxt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gdsrwoir.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qdtkjaxg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2lfbtlxkm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2brihydmu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvsdczoz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nandumxr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2jenrwgmr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nmbcgcyd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vvepfvhj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2faoifznb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hbaxixux.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hjvavubh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2xsiontuc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qyyhvppr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tiwcnjgd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2clhieswp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qtnyjasv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2biqzeshl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2fmgbbkvh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2jylrxqrj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bdulycfd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ligtjwnz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2iuvjjemd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tkcvrsrj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mnidepyp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tcrvqnhs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fklpydsg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sfbokcup.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dzujxqae.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ovwpufmz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xzlpotwt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kfckufbr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2stltczlz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2miwdhfqh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2yomkgdnr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2nhbaftwn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2slsnbhum.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dymdqsmm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmfytviz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qsnwrrkl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bfwrqjfl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nhcbhvut.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xuiotqkv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bdnkvghf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fznjygis.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sybeeilw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pdsfggbt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fvcwdjwy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jekmhgrg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gvoshrmy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gnsryjsq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cypvbtgf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iihmfrhr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hslljyjy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2oungiiey.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkodjjmw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2abqebnuw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ggpealtp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nvvpudxw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cflxuceb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yifosutr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mkgiqten.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2igygekbo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngeqlkmx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vydwcpfb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xtorsayc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qmuavwus.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dkqepxvv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2absqxhrs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kwuckykt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xtqfszhg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2llxozbxb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2glejzuhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2xvsydjkl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hhznibzo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tysmdyxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpfqpwiw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lrntfmxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovxhrdjg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pjibmtvd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dalkojbb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kbrhgszz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wovfwkyt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qmzugsby.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mgfvyemh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkinqdz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kltnqhsc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aiiypiwl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rdjanrmq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2cddylpye.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zpptliyv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gyejjxfc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2slnvfyes.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2msnbcquu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlottxlf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vuiozwtj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lmugvnxo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kmdkvuha.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qqptgurc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2riljlfik.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cjgzssqk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oxrlsohd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhyzglqz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2blyahxor.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dzfhgcgc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cbakoxyu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rcgzxpwf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pyrlgptt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qqvzdcbh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sopuxcub.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mktrykhs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjapyapb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ydgswyzc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2egelbfly.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2thhvxilu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2oqzhyqww.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qcocpwuk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2slvgvzjv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnmjyloo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dnagidza.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgqajhm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jmtsqcbz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rezxjice.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yojprgnd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nwevhxpk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2awbymvjp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yfasqqxh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2spspydrd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjsvxwip.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2embzqfcw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yqysurtz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmthrg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dszuygfd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nmqdmjhz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cbcyibbe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wztflcwl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbeciyfj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2znflkhke.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fjpnexhj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ectstflk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tkchbrhx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjfnwcni.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cojhcdzd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qgfvthhs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rqwlkmsf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cgbygudu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oylfrwqb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xevutrki.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qjbyczam.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2afhyheeb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tbqaaojd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qdyxawnm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rgeiyxfj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqwkxkaq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xxanwnxf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulfvhgec.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zdslsjlm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wlbfkhqa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlnqcahw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2psfhedrk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ysuqeqbi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tfdurmyn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aflygffj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fvlseurt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ivlqpoxr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2inntrjyc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gqhrlodi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ypbvyujv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2idkhjmpi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jrufphef.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dwdmxvii.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rtxdlmbg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lrfxulyx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fodqqgfl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2bbdziqus.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gtivtemh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uelebmxk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tsbfvyxg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qdtqvswe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mvkmqrqw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ipdtyblp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ielvfgnh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iheqltaa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uuulblhs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2eegewebv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xngclhch.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2khqfmain.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bbtsvbuf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2pldwpvaz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cbquvpga.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yjokjomz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mshvitgi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wcnrzjct.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qsrttmye.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgrlxce.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xkcagzcd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xkyvblam.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gihoqqmt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ugaetrid.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mcjuvdbo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjlxwpwc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmmccmk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmpevfyb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zrzzgptn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wonrhaaa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yvnwiejr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2aqqijeks.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iqpsejeu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ykotpdyq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cuunnuag.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bhbdepsz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2orilsrdv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ocldjpco.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kfvihagp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bwihrpup.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vbyzrcwv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdacocgx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2scguuqer.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2knggybzi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vyyqutei.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uiayiehe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hgkfrocr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eqkclrsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrbefovf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqltmfcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqebnbza.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2crwosgmm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lhssquyp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cerppmhk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2weajeqmo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvrodyn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzamoxka.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2omjdipox.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gyyjdihf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zwtrweyo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ysjepdvi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rvwwdmwa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uikffusb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsjmqoti.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjrtiluf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hbljdlom.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jnvddhck.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2snennbru.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yowytoid.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xadiwvaz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ybwffloe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2scnsdlcp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mckhlwaj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzkzjyhn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crfaluky.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2inzwiwxn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bcbwljpl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wpykhwzb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2verfrjds.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2uujjeoya.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hzxxsidu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lozvxuby.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xyqzerhd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jbfbuxgs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hbozktuz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gcjmkswi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pnixrcjt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uejacets.html


<!-- 参考信息 -->