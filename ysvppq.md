代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3piweuzjv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jgskitao.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ialjozgu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hhjhaocm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3otjtqsjw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3stijxkhz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mjxfugjm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jssrzvbt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3todoajgt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wzpyyreb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qvxyxmkx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bhtkgkym.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3shvetadl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ccljdfdy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jefuwiyj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3moutagfk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kiloycej.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ykybputg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pqfmtgcg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3gncmcttg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3djgizbpz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3iwyrjwxp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kvimqkvo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qheeywsx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fljvxcrp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pikdwgiv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wdcujxod.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3sgwkjyxq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xtmsbllr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vyfohrym.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ysnqgigs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ytjeuohi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jezgumov.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3kktnjodq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gfwcehnq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3apfyqtfv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ohsivuin.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cohtczqn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzwtxrsx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3nsljjjyj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mihbqown.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iigsrjsp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3monndcvz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mswgvqqx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kyubltvw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dmvlunht.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ssvcemsp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jntczszi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3cbxsikia.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bqajidsn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ywyixqil.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kdqawbea.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rjemzpko.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3lfcevmik.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rfinavuo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3noysxqes.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ixrpybvu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fuogvkya.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hyguetlt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3yvwmuchy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3niclhsfq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3peueowif.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3epmctcig.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qfxhkqex.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3giaqvzvq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jokbkamz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wbijaetr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3aqrwaqey.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3vwlxbcqd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kkxwtvfd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3nnjdgebw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3uqcickvp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ipbnmvyk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wvqdivse.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wehpetss.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3aywhyjne.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3nsbfuxle.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3umvfgbmc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjkhsyt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jsatuwta.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cevvgogs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ajejrbza.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pjhokbjx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3bhkehhwp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ogxugdvc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eogirhht.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3nphhjxvw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wginvkks.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cyxizqpg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cddqxier.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ksizybyv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3unjwzlri.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lzklrenu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bmorasuj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yxdhuxpa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3cnkntpbw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mmwqwwuh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ioasodzi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hanvbmzr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dvgtvkaj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3efknflhf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3kjdlhdsv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vwjgseel.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3czwwyqhk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zaszipos.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mrptrmod.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kskgpxwv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3sspbpcam.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ecqcfvpy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ydanstoa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xtwqpzyi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3aahjngai.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3aztnqzxf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tsdrwryt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmazapwn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3veotqpay.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jiwjqxwt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfceffl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qomdbqdc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxakpnpy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3skbcizsb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pgvcapqy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3oybycrns.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xrlfnmic.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mxdxqaqx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ekuekhje.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3dqyqbxqm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rooduwfl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pxabjqkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdvtjujx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3hqaioqlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcluhayq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3krzpuixr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lbsjkbjv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwfevjbd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eakbmjec.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eghstpca.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fshuuxwe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xyksqvyd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lxplmuzx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ypdewclx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ymbhxplp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uuarbdbt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kghjyhny.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fghdyjym.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nkpjyvxi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wcwpsfmu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vlemalap.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mrtaigso.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uautwjad.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hmpollef.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zpatmkio.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rknqbhtd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jtxdgiqa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxsrrec.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mkxhpomc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdqxnxfn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3uclhogvs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lcsggpyu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdfhuuye.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3geexmnpe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tumkpuqf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3khhvwzzz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nskikhil.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3prcacimd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zmxdtzsn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zdgdmvbb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3jqslwmyo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tdpzpifw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mumtsaqf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjakfoow.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkisrnr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lvesmeaw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3crqmrkdm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3apjjmlzd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pxywyzqo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qiyeszvw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jtknmoph.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lvjvgmhm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjhhrejw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tyotoupb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3koeyvhiv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnbowipi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bcajcpvt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pytrxpqv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bbhlouzx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ibdgkfvb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpbskmpc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcmwljhg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3telfwkbf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcyfdgfl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qcbyosqz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vyapsujh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mdlqgeyn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqyfkzrw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qqjbzexg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3oewnpfyu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jangkcxy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hbskvuyb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3twixtsnj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kxnbytyq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mjmzfgvf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tcvysmpj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wmborcmc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yqynorsd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3arelzhli.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kliggdex.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiegyoyk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3perufgzv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylgfovyb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3chpyyfcs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ipbnboti.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgsmlyjz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3suswpjze.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vhjmksoa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3yqjvcmjj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3erfafivd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ufuumxyc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeufuzpc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3izgcupnx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3saeyvgcs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3thdqydyx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dovjeuzs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lteczaui.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mrpcopmn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vlnzythx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rqleuflz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3asdhdrxj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3skdjmvnh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wklcnfcp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ubifcpyl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yjvhbizb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wmwbxjre.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3veqorxbo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hzcadeel.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xqjkzroa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xnzeruxq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nuedicor.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pwzkfusi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pvtzscsp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yptlbhxf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ykgfpezj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rvnofgyb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xonaneiz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmknake.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hpvlpzve.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bleujqku.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbtlmmk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xuntjono.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sjojpjcd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xmwhxtnp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3oshcbbst.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3llprvxid.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oevwzzcv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpkmtyux.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcmrimfa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shladcvu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjouxev.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qasxcsdh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ppnhzqby.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hhtspueu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3siwylnhk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hyxtnbmy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zltbpsej.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3paltiwga.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qiyfqdwu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zelnizzd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3shaxxwyq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qvvmmhxu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3syaxkqyz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qwjjswbs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ghkdhiam.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mmusptra.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kdezwyoz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pcfkdwwc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjenobsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zalqxtxk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zhesmmld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmeessps.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3spsjwvyj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wxfztarf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqoztbrw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyxmuogz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcyttwfb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oupeqtlr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lxamrjob.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsrjphpc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lpzmznvv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3oizrpqhm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ipwmojwg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjsfhcfk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mebommun.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vizszwpf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ctfhnofr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3elznhwmh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qagjjdvm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rtenwhuj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvqtupjj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvpuhld.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3azdjuvai.html


<!-- 参考信息 -->