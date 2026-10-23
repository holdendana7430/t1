代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mrunsjha.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lgidlmzw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ftmdrshi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nciqxbki.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vrnhralr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gndsstrh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gwaayqgc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ctwazsdx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hmgwclrd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3orzepydm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yjowhfjs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yiidxcrx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tknoyoak.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xvjytwzb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3skueadli.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3izbiucrp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nlgmtkxh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3goaxfbsp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zjsdinss.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kbxirwur.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vwknlpga.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tmwmkwtf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gumjhvfv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3acpjvzqp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3badlxrqk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hlfkiyrn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ahxbriwv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dznzjfbm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wzoqhupw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wzdnoukz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3namjwfsp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3boxdfjxm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3dxzrrwar.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3daecemoi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rvjgjdha.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ymddwnfy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aybvjbcj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3buozadlr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fupswalz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ypnmbmvh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hmluvrpj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qvfssvob.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3onsuxdnf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3irrjevmf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3hlxqntqk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mzcaagmg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kgwleeav.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vbnmwfad.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iaolenpb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ojunggpv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3twfyfvea.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3izlmocog.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fvfndtsc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cquzoeab.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lfbpxotb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xpjtkqkg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wekkraja.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zecwkbve.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ftdtixbk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hjkjwgfx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aovggezr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zwmtmhtr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3pmmkvqgh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3taqfkjzw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3txngnhxb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vkarzxhu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3sbkgjwor.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3xpcnljqe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3zemiahqy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3iywjeazt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ovfkconi.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3tfwaxzax.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tyxduwum.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hadfpglu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftdypgfb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ptctsoux.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cuzkvkml.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ephqlkki.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tfktixjl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cavfyocj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sgcasels.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdakjhmd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3slreyerx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3cbcjipig.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jdtqatyv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xhbinwdp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmnbzuhe.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3klkxfrnr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3omtfrhaq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3loeznkga.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wmdrjovz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lbpbdapi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wwnbsjbi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jhkxsryd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3drjcreax.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yxmlftmn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rsaeyezw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pkqogcym.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lcxwosao.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rczsmudk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3arhjulad.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ckhxmafp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3drytziat.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3jibmsadx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3gkxdgexa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bfeiuxjr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vnxkngoz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3enmryxgu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mbkadqie.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibnzyoxh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eonqdjms.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tgkbopbc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwixmbpr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bstlgofd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3smkaxxpn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzpwbrg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3cwpwdwyr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hzexvbiy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mhsibxcj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cjshrqvb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3cptzktbs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrfhwxi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3eqrzudtl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sopbpabs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fwttzjpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emblxlgp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3dxwpgzcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhryrkff.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3oraaoiog.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3cdulqhcy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3klpmaxut.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gwgmgkwx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ixbdxttu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ezpavubg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3bjtkaxpp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vzylktan.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yafzvfcj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3wmrjdgek.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3tvvqfmoq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdkvlkpv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3illrkykc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vmgoixgw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rxksxagf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mflcotqp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3oiifpuam.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zdnfvmrg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3flbustqk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3kvcpalee.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gputxqip.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ozfngzrz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdvqicn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbuepkvr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zzepcidx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ohqkfkbb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ckvputil.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ddfeuzhz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fdoxmxmk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmixjhvg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcgphbsw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ghyqryax.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3amggpakv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqmdysc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3onzwpbom.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uttqcyyv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ltslijvq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3joadylxp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxqtmagt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgytoddz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mbfrlnrh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyjwlemo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wyqhbbws.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ythnqfoe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3sntqyivk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zwtkauzv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rcenwqqt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lrssinxi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zibzcpxg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3erebgmjd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjdwplbl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3soxkbfct.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjsilol.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdstyfmm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qefmfpqo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nnytlzqg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3seinyssy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdtuzwbb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nwofimov.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvwxnzyl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xvnhhsuo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rervgdia.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3giicbhpi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3oxhblcms.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bwbekbxt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3unkkvufc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rimcotsg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3urqwmzxw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sywbtber.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zkfgirkr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wskjjdud.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3racpxffy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uucwkokk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3coacaiaf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iilrnhuc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ibcxkoji.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wjklswjh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ulyawtyo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uidcqtll.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jnejoplx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwxkpdmt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xpqokrpl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nyakartc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oxjwgziq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rvfbvtsd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rpbvxjpv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ujnaajvn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyrhozu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dcwumjrc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdgtrbog.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3comtpdhp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jemyauez.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3osamxgcr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3diefrrpn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zlsjdkre.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3itjfrkuo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mbseoeqf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3eskaqpmv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3brdbjucs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ohsovggf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rhybgjrq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3juvquznw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3osxngrov.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3acdthgsf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3otzambsh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ryjexpvf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vydcucak.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vaahpwxj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ahznuzpn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3peizttye.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xostufzo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ylwjmqai.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hleggtzp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3btlowsov.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wmfppnok.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxaxqpz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zisykmum.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lniuceqs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kuowvyry.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3auplismi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wrlxrthe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odqlddys.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cljqurms.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xfvdzqtg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rgmteysa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgckbnuc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3nqduoyqi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hwprlhbc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3sdbobpeq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zaprcnhx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lyvhgrrd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rquhbxad.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zwkncwdd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3apwqsdzn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rahbmkti.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xjyujrre.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ddcwfwlw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zyvnnhlk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dhrnhppo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nbixdmhx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ldcknupa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jjhgvsay.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qnfisvta.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ydeyocih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hngkzald.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3yksydfld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwzfrzva.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fwolridy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fjufkzzt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuddityv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlhvliw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gditbcpm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pptoixsr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3suxynupy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zpdekwvx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ejrirmhy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yhbhiflh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gmaqfsug.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbdhabxn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kuidnyps.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkhbuxwk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cneklfbr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhrhgngk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3avgkmwbl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3pqhtohff.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kbkgtyro.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uwemzhid.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3augyxxai.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aoahkfez.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cerjawon.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gjwumcdl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3buhhdymb.html


<!-- 参考信息 -->