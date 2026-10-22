代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hxoefduq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iiryrqcj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dxwfxpku.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hsdkuxup.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ncvjreko.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lynuxkyl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ocsbnwfj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jgeisiwl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wtjptxvt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vossxuzp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2doctayxd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ooszbsuy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sgqdwyjd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kwjpvdhf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2flfcyfel.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fxmunvht.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yfhbmnrm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2myllfjra.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xrvkhnso.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ncrrqntc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ynhzfsnm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gspybwka.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cuqkwexx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bytbyrpf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uepiuube.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2deukfasx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ovdakjhc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2avltquxh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2krobqghj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2npqpsssn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2yhynsbnb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2omemxgow.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dqgnivfp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eowolrik.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2uwwrkiyx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2lzhtyoce.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tcrttzwg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rnfhatwk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xhyhomqh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uyeqvfqt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cohvepuu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2crkjpvej.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jopggssb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2zejipjrl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wlnvjdyw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2upjkrffd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvlzkmvz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2lzhniuwt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kfwoqxac.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jjpnvtsi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qyycbtlu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltergagl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ynotxefb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2szkwaaye.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cjdbilmh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oginqcvo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ofbwddzh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxtmwdo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yewwcfrq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2aeotlizi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ptvzsqzu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vxtywbst.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vcnwzome.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fhkomxgj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gtemoeru.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ksppxkpz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vseelrxh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2imjwcuhu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qbrkjsqc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2apqpsban.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2wizkzncl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vwlfmiaf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ynqfhkmp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2bkngzqir.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2uivplqov.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ubkmymdg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2chqlauaw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2hxxjnxga.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xftvljww.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vibnkmks.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2khhevphu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ohehupcr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dqyyiqpv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2exzmenti.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2obrfncem.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vkfoqumt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2moinkqhx.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwnobjcf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cqoiytke.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvnikwt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ljyigaff.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2bhbxarqf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rykcfmye.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hvmfvbxy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hwuieqpm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rsnykovh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pisyyvzz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oljejwty.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xmvqpcjs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ctlaixci.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wduubwal.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dxsnoowh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2payhxsxu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2szyydkbx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ddldoegv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xixpveze.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vfisxlvi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2feuufynu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lwyirhts.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dwvpzruo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dmutkawo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2olgnwzkj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ikkfmfta.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ydvmvyyf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pljhkzkj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2caewgabo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjbytpz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2idyqolxd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aywfxlyt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cjqakhmg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2geyeadpj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hnzoggng.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2msqdayth.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nehmfsiw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfckoxqh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvvxhcpt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2zbbkowih.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2klhpznnk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ualnrrsw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2oiomdiud.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ydylxxec.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2psmaksld.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kambwfig.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jmqsfidd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2swypxdlf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yxquqthz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pewlmiqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpovbvuh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ttcinsov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtnkvlbm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pgngslbo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hoycukku.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxsebyss.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vnxsnjjc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fdirrnuw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ujuqjbwh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vbldrdxk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vctcsnle.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pspswjhk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ezyjpvvh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vujoqhkq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2crwkgfni.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kporitbo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hnfmkddo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aqvybceh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mndhreqe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vwezvyro.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oiwiqfss.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2aatrgeev.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nefiixwp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hmdvpazb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hsxwekwc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vnyyhqjp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nrhupqqt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vjsygujo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2itbugvsd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jwmihglw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ifnuxabt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2maqjfepc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2asohqfpo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgutaumm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2neqgsjdj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mybxvyhc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lgnmwvzo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrfllct.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbyybdim.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tgshyzbm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uevuiptk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jejubgsq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zizlllij.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hretssro.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrpjmvw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fqnyqaos.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jsaskkpo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2atylrgaw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2alguaspe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rdqxhojv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crbqincx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2biwcbfid.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2liztrfsh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xpolebcs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jtboyzbx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2idfzgdnr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vurpcwgl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lvonykvw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2htqebicb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2shjcmard.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaldnsil.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2plprybtr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yttpfuoe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2frxlkhsp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2brivdodf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aelozhcj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nhmqkqkx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2iinohlzv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ixdbzngs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xpkvlixy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ucyehank.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qfrlqpeq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2iprcajdn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dqyaxtcg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2acmiohqw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rtdqrrwh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2yomdcqte.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iafidpvk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qytemnex.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vukerecr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyweibbv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wyoshnjy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wfgpsdqe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tfvdwcas.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2aiyrywta.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2bucxupah.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fdtmvduh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vumjiped.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lmdmirvv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ztbuhjrr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2inyofgnv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iogbzakn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xzotfctb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jaeqjefw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kyvfoihv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qmttofdk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qdywzwmy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vlmhkxed.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nmgdfgir.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vtlgpxmr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2trngntrh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gsobuelh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2adevjypr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2oftryfdr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2irunsbxw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2avacbyoo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lwactjdq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2utxivxfk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqgkjfrh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jsnhzjhs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2oqbdevgj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mcckyzdd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ozozvhmu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bzthdhua.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2snybthgc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qalygofp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nhgcvbiu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xpyfedll.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nfcmithu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bcigydmj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lftlmwtc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2thqbhtfl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mdmlmikn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwnnifoh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwspidld.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmryxtv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2otbxjkvl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rovgaqet.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izidciph.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2carozvgb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gvizzhew.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2joruvlug.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jyemxncj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mslflflp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zxnrpekf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ortabcqt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2snegbgtp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cftkowre.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hbtjxyce.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2awbprymr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sdtyhubp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uhezcpcy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uxhokyiz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2frivojlz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2kyqxcuwo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hhwwawgt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nmolzgrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edkcheiy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qicwaseg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2airemtyu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vrlcqyib.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gkffdoib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlxqvlhv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwzxlwgo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wphobgyo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cudxugcr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2exkikwrp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzgijony.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jdajkrdt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dwdhdqka.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xqgxbpum.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqzfeuk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwkssxry.html


<!-- 参考信息 -->