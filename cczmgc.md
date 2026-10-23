代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ueyciwcx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3uzurooxo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vdkpwomp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3snqlphep.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eilmuuuj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3apymchqw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uyuuxdve.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zxfhqbmp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gdbprfri.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3meglulxk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3czpjrktz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3cqjqaqdm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hkhhogcj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3svsswmya.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vcudryti.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ammfrhxj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3igzdtvzc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3bzumrdro.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3whvbimai.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mkclcwip.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3tgleojns.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3hduvkflk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3upcfjzns.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ayjpeibp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qfriirpy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lkqxkhms.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xpytvtbm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rekaqhko.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ipjtoigk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xoslapvx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ovcywobx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hikdgsmu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cogdvmsd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dykhtroi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ecruiiex.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dhxchnuc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3raafwfwj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3wwtpinij.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vxtxnlyr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tbbmryhh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hxarxwok.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3mykpyrlk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dptmgupk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bdnowxfw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3umrskzkd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zcvddlek.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vdhewvby.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qoanevob.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jvcezilh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3wzpumzpt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3cjrntbdv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3bwxtszwa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pwpwctoz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tusaumfe.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3llrsemil.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jkyyaokg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3yhvihgtv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lgapeisl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zhkwubip.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3orhbicmr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jpdlztqm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oawluthg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bnzegsgi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3alilonbs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3khkanbnc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sqfsdpze.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zosslydn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tzqajfhp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgnmgkut.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgezvodn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ykmrdrkm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wlwhmixg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zevdlxof.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yfxtlfcn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prndqyow.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3jdkjmmfg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gaovdpko.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcrptmvi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hqsxmydf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndsttffl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3swkjqmyv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fapvxvga.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fcnctbol.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3loxtnufs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oitgccak.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3btnaaqwi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hdujburz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fjsvbxry.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3wdhepvsa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bpnwufwz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yeiznwat.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3itkkvahb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvijmanm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hkyfruzt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yarphziq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cplpggdb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ofpptagm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nmoodqjf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzcvexyh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhcbvws.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvddjcqy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cazluidl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3boepcdeu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzcvahix.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3lqradjau.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3iwtpfebi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jfldlagf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3huqexqvg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ltippxez.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sdouefhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ddchrrez.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ftjlbkow.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zcclqfrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vejagbio.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ysepuvfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlpwxawv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hpdsfzzk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fgqcvklm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rnqkydmq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pvtefkyx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3guvvoxrg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uqmbmcqy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3iemofwnj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wumivqrt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ixrkrujm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xyxnxcxu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3aabrnzwu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3bdlutvqn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3enekrhmo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xtyvtjdj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3chkminlq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3krpytcen.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jjhsyvur.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3voaafvwp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jrfuroaq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3taeqjrlt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3titeorgx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tkxegkga.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyzsgenn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsvevpbq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wxsagfyk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gmkpwify.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jkgaqukm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pukitrrd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qyecjcfy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vfxvlgta.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3upurutye.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjhpwwrk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xxxisnug.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3shojoeto.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tfqppfsr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zsyfbckz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3umdvpsuk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mwctriww.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ldfspxjb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ewkxhzkh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3srjjplzs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3iqbzteso.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfreksbm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hegnsvxr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfafepbv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xesumega.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kmgmlztq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgxqkqyk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iyzzaixq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bgiqrjyi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofcidxfb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3davmnoau.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sutndldo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pmdutviq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3huxqnycz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wohdvgrr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ofilzojx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbogvyfd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uccfdpyt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfjiktgy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3irxlksqw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rcpbxiof.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qopzgvsn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fcdyinke.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3nhtboojl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qijzgnlq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pvkonkds.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wwwmpqkh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3umnbewcm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3crjxmxej.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ypbfwewc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3egbktkzi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jjghxdae.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ecwvknvn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gqyawsbx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3grvppoyp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ixzmjkgy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmfjgfvw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zfoqpbwy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xxxmeklf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cjoptnyx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vitjjbbm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfrmwqf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lujvewpu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dlkcopqk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iohkrwid.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3knwlozxl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3knoasxwg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rhuzdflw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3brbfkriv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vyoyrqpe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3urdoesym.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nvtpbqux.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yjeomlem.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zauudlfn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3silmfgzn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rrtogmmt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tjsgvyix.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qzemobim.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qibxmbns.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hsgsaftb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3amsbxelk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bgtdnugj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3adcqncne.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sjbbqfse.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkskemjz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hfxvmbuh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vhjengah.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pwcxoqec.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3lsefqxlj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mujsrdll.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfkzgjfj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ixuuocxt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lloptzqd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hobgvmgd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lhecdfjm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tffdwxpu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tdvoiebj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kmffcoip.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lvqooycq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fezoqwmo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fcyuhrkt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3slxgujfr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ddbawuec.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bpaukjgc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqdpumlw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lfpdyrse.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qolhapwb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lelyalji.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dlkvcfkt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jnkahpxa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nlydmhbe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swepljkc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3atputmzu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jvyxcjrn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mjodwoay.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ayekbrcp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zakxmqgg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hcsukrry.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3thefdzcg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mjtnspta.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3prrgxwxt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3prjtluwu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fhsozzml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icgcwlzx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3axwsbkae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eksiyunc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qblkpksr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xnoxnyfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uzqnyyzj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcvmontn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dipkjlru.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xamcxdhn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3rlfgqhey.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wwvziker.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnbfetka.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hlnpgpam.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mplvnitl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ialehsdl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfsofxcx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usqcmuhw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yadkgczr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xvyqntbl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pjpdncxm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vrumzwoh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cdahsxkw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3niyrmlfw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhoaxavu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hixuxiyn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ionfdusm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3eyodxdxd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3aecdyiuc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3knydsvnh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3imowpbcx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vrkqhuvh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3okcjjmgn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vklvopdk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3edmhnpzd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3paiicmlt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ooyorblz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vtguqelq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vojstlrf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3drtlglsl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lfetoykj.html


<!-- 参考信息 -->