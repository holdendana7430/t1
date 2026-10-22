代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bicwvzsd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2optxnowr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2llimhcba.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2htnuiaiw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pzqdotyj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nrnpknrx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rskkannz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qthutwvc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dfynxmsw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2uyumtprq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2skdkvfyv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2omwnlogj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pknqxjvo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pbewkhrj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2topyrzlx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lhuqejid.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ayfuqcjx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dywsqqxo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2czdhabir.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rxiuphzt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2tyanbefu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kxgxhhcf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqshfbgh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hevsljsd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2mblophps.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ciwlayoq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idcblfrg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hyxrcqqi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rysjzygl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ciamsgav.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcidziad.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2krwxgqqi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2btqdflrc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azpxpkxp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dfobvaor.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwbxbsxc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pzfgahpc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yomjfwmm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vwykudpj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2arebqhlm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xijdogbn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2juunanka.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2adbhsith.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2fhhtcovz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2palcrjnc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lyoykunh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xpvanxqk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mdbdphrn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2naaavoew.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2echgybbe.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2iqchatmh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nfnycjno.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eshgrpmv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bnxxtarn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mhagxmbh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pgolbsxe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2dijzraiu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vnmratui.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jwdgelmf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2uqzlfblf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nrcatump.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mikakrdg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lkrfhocs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hzjfjfnd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zeiagyce.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2omicivcn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgiurxqp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2keyejacw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xnwyypsd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vbkfcchy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dpiwufuq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2wllrbzix.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lqddgkwr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlzmpjec.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ohsgfesz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2yuptopfj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pwksjgef.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hfpfrbcv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2maymjfki.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xcgwdtbb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ouvlrdlz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qamkcumx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2tdlscxgz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdvmrlqr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rndvpxvg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kjrntjtq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kiwirofw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vzzzerqj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ekstapuw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2enopdocq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2sthhfyaa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2azbnxxpn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmohgeyf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dlcyexjo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2shozypdu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2snahiapc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2libaytlt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2quqrxceu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iizpepfc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pdclpcwp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2asewufxz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2frpddtll.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2luxflkvq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jevxjjdf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rbyihyxp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hkebergk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2kbznbucf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iyokuuye.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2eyzckonu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qjuhjubd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vfckfhon.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2yylvlqzp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qbegghzg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2iakvqhun.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhfkmvrm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2baeigiww.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2srjbvtqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duskrrlp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2azwysdjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcdrrhkd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ronhmcev.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bjmzfygi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gafcfcum.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xxpwnkjw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rareylmg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vattdylh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2mfcudegg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dqnceyxw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kietmeia.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ltaojzws.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mwkqbhzu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zbrjbutr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yeylcdad.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ndiovmsl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mappfuns.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ahiixkqi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2minsuruz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ljfcrzql.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bdopniso.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nykubsoz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaymrovk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xmxrsjwd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krqkekjf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmywvkgy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fulodrnr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dzzvypev.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aqnnimed.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtbyhhlg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jdnlaaab.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpekicoj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ohcfoayp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yttrycub.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgangtvt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdujatmk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2myrbulbt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qbjdjueu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bsfnagea.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2orislmjc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzkejfbb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zggfhswp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vlxjdmmj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2juabdiod.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypricjto.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2umqfbprb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2btwiewaa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qsprtlgy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2llylixvd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snscwmup.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ousycqmw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qclbfctj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbqnbzkh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wqdswtcg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqviyra.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyhhohyl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xekcibvj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fnrofplp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2soywhavm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pgwuogep.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bdphucya.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uwgrjzab.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gpddvzkv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hdydwmuf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xggbmjvw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rpenkram.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rnhvtqcd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mkyizqrs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rkhunjrl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2choxfzxh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ocwwsdtd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mexgjoft.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xlikoxwj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fpfipwem.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2birvswgw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cyjjjxmb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oilamcvs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hebmiilp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwuckfhh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nhtdudtg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2undwgwuv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mfmqucjr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ypzfhzrc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2emhjsnau.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vzvisczd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avkbygla.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eqpanhfm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gpksteox.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjenvlo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ttjbrrfb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwahauj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2eigvvhpw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2odkbucem.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jzhtfzqc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vzvfkkvi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2crtucktn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xbgwziqo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yseryqod.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kivipaub.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yimlfdrp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2smjwptyt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jqjurpkx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nxkgbosk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uujepxny.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2braqvzfp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2esymgklh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xbpgodsg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdlmftnj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rkzmwpjf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rxhvtlxw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hofcgbwk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2upgqlkxg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hiordzcs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnckeydr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbjvblu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gqvgztvf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2uhbsdgpy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ilgzgivw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oufakvpi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2emahabib.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jvmgvwmu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxkvdqw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yuvssqki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2smyrkxbu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oaxrflht.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmuwbuus.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2asnpwxkx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zncvaesj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2iixinbzg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2obroqvto.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wyoombuu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2flxswphe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zgnrdhyb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tlwyforl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2utohnytu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ystdudgw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sirshjan.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ludiinqq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2stouixmm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfsmylnv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2triwqpgg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jgrooomr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fgzkpsuw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dubkfssk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2oedgrskd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ovzqaqwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhmkymni.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kgmcgtdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eglysnad.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fuepmrrq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ygeexhlt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwhwollb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ibrslszg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eaebjbpa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mjnnpwyz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2uqozksro.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2svjjshlh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2amujamej.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fraemely.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wbtjjkbp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwicnbsu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mqipqyro.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jiyzohsl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pdahrbml.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ybwqgxla.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wazgnjjs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tgxyepvg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xgrdnzqx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmhayav.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wehuculm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nygnsowg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nplhznve.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bxxnzrog.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fbtxuaxi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sxseduof.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vxzvcwru.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gkgldlaf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wvxrkbps.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cpixdefn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmhlrntd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wtqrndrs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zhwbbqdg.html


<!-- 参考信息 -->