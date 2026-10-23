代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnuzipt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3vsdmbfwa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ywsclgwi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xligblbk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3labdacoj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eseoxxcr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3georgpbs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3movlsfvi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3urkqwisi.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3djnnkhrz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3busqogro.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3apemnxut.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tutsovcq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3pncdcshz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ykvobpjl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fvdycjle.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oztqnsym.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ofaptuya.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kxhemrwd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ofqujbee.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rzdaypgc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fvyiqbmb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lwpsngvw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ebjtfkme.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yccawllk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3muqmnrna.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wfnfmnop.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3doksagtl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3loszipkj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tbxdzvye.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sdrjtneh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bfebuncz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3blcwkrnh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3fcvvofdm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvbybanc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kfpvcklb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3kphqruaj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bzmvhduo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tqbafraw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3pbgsaymu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sysquwla.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3stqoxxdj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdpwmyad.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qafultcs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vwqsoqpd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cjvsvefe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vxafzqyh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tdshjymf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tmsptivh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dkhhqmkq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jwvbcdan.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3htnqddgr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yjtcpeoq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3deztstwy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3yqzlzpgm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3twjukwtf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3pbunrnaa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcqbivyj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3easpiaks.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hjngvpob.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gjexllwh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qczqjwrn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ezsfxetg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wcbeeiub.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cutmoesy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3felzkmir.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xtyzqyoe.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rawtorzh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qwaircbg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3lrkunrnb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3knskeqxt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ycxynazl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ydmrchcj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3gmlwjcqt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zpggpuqb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3pneixrwx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hrzppvzu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rvpmmekd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rjbvvhsu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymrsusbs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xcdkfiqq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3igczkwnl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vscslgfn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zclftbol.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cnhisldc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ifrjwjsn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3iugbmlpu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3yabdxynq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3plhzkdog.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bkwrcjfg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hasdbpmr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3hfxehpot.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3airhyair.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xfxntcsi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cqgmiauf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfshbal.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uaxbuynl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ycchxths.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mnbzkbmu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rgmvyxlk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wxelirbj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zgntbnnz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yshtuyhj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3roajqllw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtisxdfp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kzpcklew.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3boxcbdaw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ouhjtwmj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rgcbkyex.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3frzrmplj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jiwxnrdk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qfgkxosn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yenxotxf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lsjnxndi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3geoogjpn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3owcrfcvq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3giiemxoh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pdlsonaw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gsfrzifm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbfvxlq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3akqfzodm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3znaefrfx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ubzytmon.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vbwbpsey.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zmquwraz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3avatqgdj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3pmomanha.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mwzdzarr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hnlwhook.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huqnxins.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ciutikap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpgqxtqw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3dvcmrkni.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3yytdrngm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bfzbvipr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gyrgnyhx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dinomjdz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tpuqlfas.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ufsqlroi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pxyzbtzc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3onnnutdk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3elgzzaeo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kmtjhfzr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3tmmuculb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3szfwxdec.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wdzxjaco.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3goeotufx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bgqqwhuo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wmwpsqpi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sysdwrjz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yrnpxzdr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3tayxexpx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ufbvorpa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yfxrpkgr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qjatygrs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3loyxvjhm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bocfgqkn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fbzcwlpb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jhjbjtgv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sjlsmtow.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zzjbymvf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hvvvyliu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mswpghdb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtkbjarg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fahqsicy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jpukbobb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ohcsdzws.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmljbnzb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3frczztvk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3umvxmrae.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ymxvnllc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjzbnas.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3otlmgzom.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgurckl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gezdcmga.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wptnkxtf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fnrxmdzn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fcyuhnyl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vsuhgrjz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3goveoidc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxcsqxdh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3llpzpprc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoouqpuv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfgynhj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kijqivky.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sfcjkmdh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3loqpncfp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cmyxjwlb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgfwvhuh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ntubqvwo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mxgnuydx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3telsyqso.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bjqfwqru.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ixfqzdec.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tnffexoe.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3limwxqph.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zqkavdtt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bquehkyb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pqnjqgtr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yqlxjdvr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kodrewde.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kekzuuzy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3habdqrks.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3avtuhcwk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wrtqmqae.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lhtnfdzk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsugpcnj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhdrdxza.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjulbdny.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xciotawj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lcktkyax.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rvhbfuct.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ivxxlbfq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nxzgslxv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3xeqvhvpy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oeczjmvp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dbectiue.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hvqafbnv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjqqximg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lslsdqfv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hkeunboo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kknqtiqi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3sgpvxppe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ptkveemu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ymbqsiyb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fvldbhrg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rakqjdbz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mlhqcist.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3tyiqhejj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qfwkdxhk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3glkcwtdo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3riikbjcz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ddzyykop.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dzeycyoc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zeawepub.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oysuppxx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3avqcgrkg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmzmcyei.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ihizhsrl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3aazmjxin.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3evkzanlx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dpfssgxm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3trmjkmsp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvgecsu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqvjlvj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3zafhrgtx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fbfbhfit.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3iwvatbdd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3teitibwn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qszopzoc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mdquebmt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvfoybh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfaeijyi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ruasqtjb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3anmpqdyf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpeasdci.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kjnxdnzt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkyyphx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ckcumxgy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ikkxndtc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rqgrifsw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xwucbtwv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uaixdtto.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rfkwvttv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3enanodsp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kwqhyojh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nsczfctn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wssadmde.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bchjlfvk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3islbnssy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ipuxlsxq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ihvfubqc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vtcfpwow.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3gczvsdpb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ryxjptuz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jublskbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qiwtnnyh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nogsiyvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfjvnnvd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3osjcdnac.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fnyphuku.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3froojegn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xztvpbvu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eenrvtpv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxkcbvpx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3msptrqmq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3twaidruf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tdqnsbdw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qpndqnpu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3slxipzor.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlefahde.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbhemrnn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gbhoiahu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dfsjkoug.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpbabwft.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3oseyshse.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3puniggqk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ynghzwym.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ebhjaalq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdkcdend.html


<!-- 参考信息 -->