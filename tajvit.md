代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gljrtaoy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wrkufwkc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xpljfvfz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kamcenze.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3emiisvvf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3igktcsvv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yjrtmlua.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hqerhzhk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3pnrosukl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ftfaphum.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3houiorib.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eezfabps.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qzmqfwck.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3nwuentxt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fnhcgpkp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3mglinkra.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jeilcbyp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3zbonzhot.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tfllelai.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3taznultu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pprunyba.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xxlmshbp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3moqgdwar.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ivztrlgm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tlyenihd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vdcgfrzd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vtlckwrd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dgptzimo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3gvhipmzu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vmdxsztf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shfkkpnn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfdymvbx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3znbmuzeh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ppjvsvxc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujcxmwdl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wuhfllqh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtcguflc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cykbdhgv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tczmvxfj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sogynlqn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pyaezeqp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ocvcabgt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3opxqcdxf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnhcmdau.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3feqlswwp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nptrwtyz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qkexouef.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3auxazfmx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wkiuojhm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vhfermjt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3cpdssizg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ewuaikek.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hhylhzqd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xqqmtptk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3easeyeys.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fbavcyvp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eugxkaay.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3reyqosmj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dekkhytk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3shfmdyel.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tdzlnsoo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bwrquzha.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3seygsnbs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3dkfjptcm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lxthdqvn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ymwjrsiy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ojvypkoj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vkpvhqdo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3gyrtltaw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dxctqkmv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3elmrgtxq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3bccszurr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zmfikhwr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mqcemeli.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eulxfusd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3saowmfms.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dvqzqdtz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ithmyjzn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hybrpamq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ligswymm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jjebkbuo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ivtzoupj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ghupgtdu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3nekfypzg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3utlbzjzj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gdgvmcad.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3wgznejgc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gwponifh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3onbzcfwc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3knelpopm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jcxhfyhh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3orjwcrcw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ivkdolyv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eajnfqly.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vbdaswoh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkefqjff.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uoryelmc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qauzdaef.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ufugnyrp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3znddqzyr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywzustkj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3riwerrqk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zfopnvqq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ybhznbeb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rdszlmud.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3dcwhqsgg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3feapcdix.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tdfdhpyi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3prouctfa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3htnbespt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vvjvmjqa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hompbryq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpocfmka.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbzcluvl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nqwiowdf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vxlujabw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ndxlzsnm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vayhthnp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ycmzprfp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ewsystyf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3aikjxtlv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ossoxuzo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3htfozdnm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dihmvsbo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ykrqsdyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvkanqoz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qbslbzvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ummxreqk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xhiexqbb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tvhfoibj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lbisatuz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dbnqvxle.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kdmtafen.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lqzopxep.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wpejbrww.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kibaqbdm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pieupkfd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3opbuuzhg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3drrkgzag.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3yhiojqsq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3comupcjl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gxlopyzy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oubcyvoe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wrmuumak.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zowjbohe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vriqzjsi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3stncijum.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3diryeubc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jfrsujsv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xoseuzau.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcplfzfq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xriahlcy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rrkerxxd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3imypcqkm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dchmcgan.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bzstdxhp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fljkktyh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjdjvamg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ckndwdiz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgjcikk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3metcksmq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3lncsjucb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mafhnpet.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoialtex.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kqhxbhna.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3gssytord.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qviuihdy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekgxdhpm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvvmllsh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjdfdijs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dfeeelhz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjlohyh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dbvaxdbz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nlldmctm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfgrmqy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emxtnqyu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnmhpgfc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hpgwyoef.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuvloskh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ufmmsmfo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gzyvwjcf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilnojgdr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ilzsftpw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3algllpvy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckfpwydx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhjazbwz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddzyshyc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewnypucr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qdydyaku.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3owmrtfjn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyvuseql.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vtfsbpwo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3dpsdzswg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xscxoexc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fluvplsq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3crrnkfii.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jxdqdcbj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3movknzkn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rwnnhcga.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ijklhukh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3anuhammu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3toshnfvv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyrwhcpu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qdxqboll.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3emfrqvpc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqedpldv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jdraoamj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lolcxjyv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmxqhytk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3desnxqca.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vkfqogor.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opjldyru.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fsuzgjrh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ryilzxba.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlxolrkn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hldjkzxs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gulgplhz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cyzjvqkn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rnbwulrk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lcjdervj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kfsazaiq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pvgavoej.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3guykmfja.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vquanzhn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mknzbiht.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3smybbyyx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cgxyarol.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pnokhjue.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3nztfokga.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fxnvqxus.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ftsbukng.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fxjbjlti.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3alwujbhi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xltdoiei.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qfpharff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tvfjitqy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sigmrsnt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3efcwgack.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xqsoervt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3studvwiq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vrstojot.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3akscufbv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hdojfyhw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wgwqimkl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qvshfejo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xsxkumqp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qbqizykg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3klnmmpfm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekuagfhu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zicebplz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bnhjoqdo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rraivhha.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsxtdrxb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqcvnazi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3boefomls.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kwukgymk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pgxmmalt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iupvwmcw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tupewcoi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3psjzkymb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fknbnjwp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sxwfuroy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ucrpnkce.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zonigais.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3sgbvfboa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgpminhs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hzocwugf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aqresumg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lncpuyky.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tpinoltv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xzjmhrip.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hecoacls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmgugswf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ejewsmmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbgcypcf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwgyvwps.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ehbhdszw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obywicwf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehdgrbds.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cguucwwq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wskzkyfc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jtzcwbzo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vmfnrtoz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcqavoqs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvpjegbs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wgmlmdrw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpcechsu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qrujswev.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fbtmqxyl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3huepvwrm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3otlsqezn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3aonatpxq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yjicfwnj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jyiknixp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ugnxyfml.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kftyeopy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwxgmta.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aoqkaxrp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3idneetlr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ciblsxgj.html


<!-- 参考信息 -->