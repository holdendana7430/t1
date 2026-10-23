代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qsyvkhwb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3oseaywos.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3thqwldlf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3tundcfiv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zmlixqkt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eifvbnqw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmczqo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pfcembul.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wvdzkuvy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qkfwzxtq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yordzaha.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iubxomxp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dokcnoas.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3itbbznjm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3comwaqek.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3erqbonhz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qagxmxdn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xrjzbfgl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hcucwgdu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ljdoiztu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zmauoyra.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3isalzbhp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ejdfxday.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vlinntri.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tgdaghtc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qvrkmzps.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3appfpxrl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3lckdcbwj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3klocnoln.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nbngfwcm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3laoqiwmx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qusdkxrr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3gndxsrwi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3mdhmthlg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3czbxrciw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rozuhfns.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3zkipntyh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rorbbywo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hqoztjmx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qkvemodn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3krdjsuwu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wvonhwbn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jpbjrbdg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3txdplkhn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mivbucfu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jalpubdm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aocxzhxx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bqawlwyx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ypuoeuhd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3meyyjmpo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oyjyvrbg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3pqipcbkk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zlffwmrg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3iczqfzid.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3mgvhfzya.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3judjuhzm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gwpbmwec.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3rsbzrxrj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ieegqsck.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pkpmaeiy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3udgzolds.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rtvmqjvp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3nqycdeoi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oiavbana.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ehdmlzyh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jziyzmsc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mpzebujp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3blbbutoo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3xrclhvks.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jpufepew.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ewpyzmgr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3oqqgxjcj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3trhfpkig.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ojyhxhek.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3puanhxve.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3imtbtgfv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jltskpdu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bmkujtbm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3glutipbu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mapkoekn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lvklfhqb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3igzevqtn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zbxtminw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3unokpgjn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tdmtrvol.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3svojqxmm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3lbdnhlum.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lhsabvol.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hjybcoef.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gzkqkrzc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3imntoayu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lmtuthqd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3duhifjdx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ydrmbobw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mobgyshf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3scwttoxu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fsucahxc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3shbzxxxz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lvfuvvuu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3acidphdw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nfbslbgt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3kvqrquio.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wflnbogk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gembevkr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3eitdszht.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tfsxjqvr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wqlqvzdv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bkndaxmv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3onatthvc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gqrfivui.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zoomsszk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fxlhpuom.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3wyvensxd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xayemwzy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckppmpiq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lragjwji.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3quymaobk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bpntymku.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3cquykapi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oheqmhzj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wdtwcshe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3fbqbyqfx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ljjprymm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hmfygeyi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tpzqkama.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uawxasjj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3oscskjzv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cwafeaka.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jdztsmeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vktnaslq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3huntiheb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbkgjieo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3tagmivhr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lhkpazbk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqccqasf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pinepnhz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vpgysaic.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3exzpqgat.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3plegvexn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3suxhygqy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qscrrpav.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3siawapaa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ijwbzotu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zofdegko.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nplbyxjv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rpdljvhl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uefhpuif.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3okssplta.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3znbiavsf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cxzdtnbt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tgitcdht.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3owvxumoo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3klpotkpp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ndrculbe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cpfggsnp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uldodtmv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3maffminn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jxqfqoqj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3niwtvkfg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ywsbrsng.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rptsrjil.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pusmvzov.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dacljgoa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmaqtdmz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wtffvkbz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bhrjghzw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ozlzbggz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gpfivznu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ixxosidk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3agddrwcp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqvspkrv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqnkrbfg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zkqxtmpg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rgqiqvmd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sorvbtof.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3odymadeb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3llrxvpbd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ohlcgdkj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ugzalnfi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vvjflboi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3blkootof.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3docwcqje.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jwjusdrm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3grlqyyam.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fjfvktlf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkjqjzel.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vjswzuqr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3amrfwtix.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnzspra.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3revoxaxe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjbumlqh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cqflrzst.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rzxqfjmb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3azeimcso.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sajwrcwh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nvlqrrhz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xkvrkfml.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pyorhifr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pkzlvjui.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kcsuyctq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vvewaxos.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrsaohbw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rmapqarh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ukktmape.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zrgwdzzx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3oauyqnai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ymrirbxy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfzeyafe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwpvifxd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lmwobdde.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxzasnvx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3offhrllh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3neuxqowi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xujmwqml.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jncbviko.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xruillko.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3skpswypc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3oqlbrujr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3twzqreza.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gqugtszr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3capqernw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3moarkhcb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3iizhmglg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3undtjvpg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3utxkzmdt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bmmfgxjn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytnmggpw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3srnmhmab.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3eyimglqg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qlymjtjy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rnbuyaky.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jtodzzrp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tqsmetal.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nihvekyu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iegpkksp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gpctiqhx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ciktsddy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zdajogmn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3trlhzazl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3oeqqpouv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3tsmlycuj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pecxgpai.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3obkulwpm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcotostx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3awzwqjyt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hiqisadp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3nmkclaco.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3knkjklvk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rzvgclhk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3trrsnzzg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nkjwdhiw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wvphqhrb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvopzvkz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqehzsbx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wjplfkve.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkxhlatx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lhcfvdox.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3txfvbtji.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vcppvqil.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wqskslwb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3scwpffxm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hethiqgp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xupkseyi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hxqrieyt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vxiywmzs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3czctqmjy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pridobun.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wjrxrrjo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3drrlpkng.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvqsosas.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bhteiwsk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rmfthrjn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zziganie.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vwsvnszo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3usrvneec.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ejdqxkxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iomxdhhp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vkqsijnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvcuogoo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ngsozcah.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jbxfmlux.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kvzfazbj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfkpgvzs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uysfkiqi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3apngmokr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lgbxlxsj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lhuyioou.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3safehzol.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nsqrhlqt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jgfghfhm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3isznoqui.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vpwfqqnj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzvtjxda.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fbiozmfo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdltqgtg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3urcuktrw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cirpwwab.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qhofhzee.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ylrpprlj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pilqohec.html


<!-- 参考信息 -->