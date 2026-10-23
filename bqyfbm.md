代发 wailian999

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ckxwgdao.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qfooookb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cpxjssgn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hxbtzoai.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lipwqcbn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3mcdpwujz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3keqlcrmq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ehqetztw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nufzkcxk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3echzlfbq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zvfwebpf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3urizaaxf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qjpwcggh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3krrcwfyc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pwrrbhgk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3utyrdhcb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jwefofac.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3deajmnbw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ujrrdqkd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xjkbzcoh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oimnrsju.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ayflqdch.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dsxeztwz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3crynmyak.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lwjojkbw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pbxqslyn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvwipugo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vtelaxnt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rrgrhgwm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gzadohyh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usabsqof.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3magshacg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nxcqfoyi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmifpvjq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oviqtmkq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eikpzoyt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dgdkxfyt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdkycize.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pybuurdt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxysvgwg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rnwxxyje.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fposujap.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3luoovxjm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3husoxywi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xmdcuniw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3oaznqxzn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3syxmtsxg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3kddomcwc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vnfxkvll.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3imhjwsyi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pmpamuwt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3epfgpgor.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pxdjrday.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3isarlczp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3sdjofykc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jgzfiqgn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3telgaxtz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zoqzjfis.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3zsnptvyj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3lfhadeal.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ujjicmah.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xmutemck.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sqjgythe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3emjtvobv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3susuzuar.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3pepiwval.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rdsqboqv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3txhpehch.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rooulkba.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xozqjfki.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rocevwav.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rkyszcwj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsbddmk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lwuepese.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3begojtaa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3uktdwqlo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ulyhhxnm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ezgdblid.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3usbdmvgu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3flqakmhx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ehvksrln.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gqoixuqt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csunadih.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynkicmxd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rirvxukm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eleecsly.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xcrqkdyb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3bneddrsc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pwmyuwch.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hwdptzac.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ktsdxeal.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rqvptspe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hkjumrad.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zrrlyshj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yrqkskpk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3neeqhrmd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jerygqde.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oeragcoz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iemedkpy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3zgylvjia.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3dvphegkt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bqktnknb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eqhbktwu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ktlwyqgn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3aregnlyl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uicwitue.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxujrbvf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sdangtzb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eogbsnrw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3idgeddop.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3preayqpo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qziirhuu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ryczbylm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3umksiqbd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqlvoce.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3bmdbeqtx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qvstefpe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ksvcdpct.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3slfmjfdf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rihovqjq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vmutbkyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhkvbupn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3sfjnfokt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjmlhomo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3geumaxvu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ijxfmznp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgtduwny.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oltbbhxr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cxiwpwdt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3onazczns.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3biujpmom.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tmyjbpgw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zvevavyc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3wxwbctuv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3evixlfch.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gykuixax.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wdxipsgw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gfhkdsja.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fvasubyn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gfaryikk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xpnvmdfj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jdkhpqkh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mbffivsl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3klzusjsa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fqebiewa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrnbyjyk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbrxxgbg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqczdhin.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ccjrodfs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3imrrpuxj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cpgtotma.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qkyjlned.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3bymotvnc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gyfkdtbu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fneheqvl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jodfaybg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3systxnui.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tozhnrot.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pnpekoli.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcbihyla.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mvltnfzc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bfjoltot.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wpldsvdg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sdqltlwp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pdbgrnve.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jezvrabj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3frlwynfp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ycywsziy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3owufxeqy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lsvshdot.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rtvzwqej.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kxtudhdw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tmubndlu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3erptgbac.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3otwcgybt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zylvjfcz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jtodffcl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovbdampc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kagbbehj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xsusvunq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gywkyszp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqumhfbc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3njemjelr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zegilmby.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qocbsgxp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3djgfhwov.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dcxfohzr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xlymoqdu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yegcjlbw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kzbiatwk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jgkghlul.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qlberqld.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3crwzojgu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ekymqxpt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3oxcmramj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wdehwzhw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wvughihl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tusnsprm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cyxcdghi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xvylxogk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnkvkgl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3chofnxrv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tewrmlgz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hliqamob.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccsiqewy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3idfvxuoq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cvohszhd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yshqctva.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rvgsjyft.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mpoxnwnj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3glaiyxpa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dggbxvna.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hglgbpwc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wctgxziv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ehdbuvkd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lyvidaza.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mmklvjwu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zflifztv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hoyxyogx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hptmfkuw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lzdwfcsh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lolekuos.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hifkrvtc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3okieigci.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3iyrybtef.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cghucssn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gnohkggr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xekkjvap.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jypjypsl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3eovplyhl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gkjlmrby.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3axpfpdyu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3utfmemjz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zcpacjjk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cejjynld.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3foulkxqx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3luqrnanl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3zpmwrjpz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zfefwljc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bhiwdhrb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rdptmjql.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3svngwmth.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bpstowvh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xjeogqiy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtkvmram.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybfwjxkn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cfvmabwe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvsnnfjz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mivxgssf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bvspvkpw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3drszmvbg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3iboenpvi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3osjidrly.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gylcnzfv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zkvdpbfh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yncgklav.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tsontchz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dzowqxfn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ytpdijjh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gqyzverf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zrcnodrx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3inbmohzr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zcjkuzxr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jbmmjgoz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jeqoepwf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhtqmtw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vnssukul.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3snmiofnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htihcdlc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ugvakhun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofzwbjys.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ganbfktu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kagyqzta.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3owgpxpbm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvemufzb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gjxuuzdu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bifdtbxm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yxfbozep.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rogcmjbg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjzswgvn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rkjqpfvx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fquvlimq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ghczqoqu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgyrmdhp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qytgumxv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gqllibdw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3abfrumyz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fvgcimdo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ghvilsse.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vkieouyu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3sfiayuuq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lvvlhrkq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbewuqjv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mmrhoayc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpeassqi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3znezbboi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ubqstmlf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fnjdctom.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3clwbotdg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vcffjxlr.html


<!-- 参考信息 -->