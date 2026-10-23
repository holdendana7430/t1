代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wsindmui.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3iwfvijby.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bngilfmm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mztksumc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jyytpamy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vdlkfzvy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3umaqbzcj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jygdterm.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vgtejxkw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oaiupvzx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nbgrbmkv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eldhnmgg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3anjqowjg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3aqhumkmh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yeulczsu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rypdzksw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ldrndkho.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bgcevyeq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jqzydakx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tftmufua.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zqniwori.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dvjhqdxe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rigctjsp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3amffwsrm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3emwofpeu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sbdzaoua.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3vsthbyvk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3etjtiaiq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rzaxqmtc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3phjjvmcq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tshffcsq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3khsmstkr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3omgtrmcz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wxgbbxzg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kspurhuu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3wdwsijzq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rffjpgne.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3objzdcil.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3maeymvrg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3lngaeitp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3igdqejwy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bgnpcfjz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cszlnruv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bflaalym.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rthgpjcc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xxnqfqlf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tgntrnhb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdyclhtq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3dwzyabpd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3znkrzeww.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlvqxbl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cvpflovu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3snpywscl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ehgnxmsu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3sgypnvrz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3owytjetl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3wfwtexaw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3blkeopco.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qeosjmfi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ytuldhnl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3imbanlcc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wbhngzxp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jpiriagx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vlvqwosh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pixfnjle.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ojojwjbd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3nrovdevx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3sxktauwm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rquvwymu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ybvpvgyu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3juvokocc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mqeyifia.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3jscvdkni.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wzzdeoiz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3eiruzssf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zbfduvvj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztppfldx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rdbvsvuh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygvmgssx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3waqoifxy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gbmwpema.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ikrahtgb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zqychfnl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fznysryn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hzzkwaye.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibyummti.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zymajhds.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hmfuycar.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bevcayjw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3kjdwvndr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3cwfeztlz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3dporuhty.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3lwspxznu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ddzqlzhs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xoeueoik.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lzaukimg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3migsdxuk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mkmjjfvu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3asebccus.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zlvwdfjf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3srsdjmcd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rguughpx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fxkfwokw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tfjudelq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyihavry.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fvstmbki.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kirvbcyo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ukkjnibj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abvqojjg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3clajjqqy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kjpimrgd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3viwvwruh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fgssejas.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rptxmwgk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqciyzn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fubezyoe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3znxtgnup.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxroqpl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3odgxssfc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxdbejyt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3pgnfbmuz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hmseqaqm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsjlozl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3asvsvaiv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3akneckfj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cghwhqdc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fvnxjtqo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vgtmuitk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gceseblz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahejebsl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lwvtmkab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wchqalqi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rdknhbsu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rrybyjdm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zzorombv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xzfmdpyg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qttllmia.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vcmjymht.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wdpzywxi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zbqfbltb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zvxbadio.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3whstvtsu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xaqzqcci.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rpbgnxli.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gmsrmcdw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gwlpcxqo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gwocqjwo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3leezbxir.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vjcjafvv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3divjzuyg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ybqtgvof.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3djmgcxbe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hxrpkrdj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fltemijr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xfruhfgl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cobcfyoy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mcoqxezy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ybqjopox.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3abuuujju.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cdvrygnn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gekjtbml.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3eeuhmvlv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jvyegmoa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nlgslwiu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rdgmuelc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3aecwldvp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lsxwquoc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fzxwnfix.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ppyqquxf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3yqievzrk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbqwfrmy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zehasvld.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hgcuftbz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pxwosudn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3wykntzvz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ycrrjzlp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoenmxwo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3frarmwgn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hcxnjowa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3subbamik.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zykyhcai.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3toipvycg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3izpppgdp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cjwjkvoi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3quyhyysv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkarllu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3purrfgri.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ggkepycr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ixsgryom.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hhmpelwn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xozyqysj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnrupogs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zmeqwjrm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3iwzzdese.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tbkhzxgl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rlhemczf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bejbmlsc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zbwwlpeu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gqpbtuic.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3focnzzjv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aeqygprj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fobvgzfv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3cqmuhddt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3drshuxgs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lxhnsmqb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hzfaaaqy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwgmgedg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ixoqydld.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kxamieac.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rqpnrzdx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3htmwfkzp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xnqhafti.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwsfhakr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3okbgpazr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3yhdcrkio.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guhhtgdr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3caupxahj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nnmmdlfw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mygrdrht.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hzlgsuwy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qhtohogy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wbojuobd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qjoozmem.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ubgiesnf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mlhmwtpl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qtfdnouz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zfcxwmjo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3josrwhtc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ipbdzfnq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tfvjreoe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tolroijs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbfxhhgd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zulyrizl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wakgmcrt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oesrjmdj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3crwaltkw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ndrxirdq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fvsckznx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fhjlmlav.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eztzxzyx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vzilnbty.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jsweebed.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3aepxjrjj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gfbirfmn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdyyrmcn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3shvclmap.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3onoioygi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wevexete.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3uwthnbgk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cgfflmri.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xffyjbwa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3awemybhc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuwabzlg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybdmrfel.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lypfmxka.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyxazqte.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmhfenq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3smxphxaw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ayzykfne.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pmbhsgut.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3raiwjegz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nrvrgjzr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gamejqef.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3riicbpff.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sknxzarv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ttqnnvwi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3whtjxjff.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xlqqcecn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xxivgfok.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwfssjmp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tnepznww.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3srchuioy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3myvupzhl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fledgupg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3oicqifms.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rzberqnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3migrqzxl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ioodlzqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqcwzqlc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cuheffhm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wfewpfot.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzazaqfh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xgxlcfny.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ivgkhbcw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnqwuhco.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3atocudwm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpsddgqm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lkftxeou.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmwiplbq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3opfbxmaf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kykuutbj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlbxodog.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btqonwgy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vqzvycti.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ugolevyf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bjfgorsv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3chuqqust.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3crcdzjrp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vmubagzp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lzrwzqza.html


<!-- 参考信息 -->