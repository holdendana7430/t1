代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wtzapcjp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yzmrniax.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lwzhnppr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3hjlkizep.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3kraqjggh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bbvldccu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fyruecnw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqldgij.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3odcnaxvu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zbijqurr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hnbrdbaw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jzfhkxav.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rkpojpqf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3npdbohgj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xcqzlrxu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jnuofwhj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jeokdrms.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jcjtfoaf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rbnimrtt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hmvcjwdh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lmbniscz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3tawzeukk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nmtvausq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3itubdtuq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hvxcppfo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3sxdbwcsq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wqyvzqsn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3biqoqhxx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tqiwdocw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fhwmxavz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xmhfowjq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ouajrbid.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3daqixxoy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jqjtzmhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3xxbgeiov.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3kizobmum.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hrpynsan.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bxceylsx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ylybkmfj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ndmzshka.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3owrdfzqs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ybrebltt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pwgxurdy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpjnbwhr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jwucwziu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ffhibajj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xtylxeqi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hdufxgsk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fhjoqymi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vmmldctp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqedraxk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hzccsnrz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3suoprixn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3guolxoez.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dtpknrti.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3holzzyuk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ldlvjslf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcnfgiz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nijvfvqq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3papheyht.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bqquvymz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3eyuispuw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3kyqkguek.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ahlyiiob.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3zkdplnhd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3puopfhjy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hfvkbgyu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3nitdtdbh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3aklfkibp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3otogdmvw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3aaqjaoyh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3twrmbqug.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tcdntydu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3uwzmzhgn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3upngsjul.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3qkwpvviv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rdlpitvm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rpxxsule.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ysprevzb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hjusuhcm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3cxxvzoeq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3uqymjahr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3hexlogys.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3nwrkmveg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wpprogem.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kokdoimu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rqngcepg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bkosuxnv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zdpdmfdk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dgsqvuct.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3szooepni.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3gnnhaslr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dvvbpfle.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3kslsghqt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3pilqgrth.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3stmkkyfe.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3shlxrbwh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hktqbxor.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zozooymh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jzupvncm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zcoabqly.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hiqwodcy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3jkldilnv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ybtghmrh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rzjupyoy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pharosxn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3heolyyqj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dytaddap.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nyrcfnnf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3oiaslrkz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ypdgdori.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3mkbhdtad.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vmhqweio.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yojdziuh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3risatozh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nmsxfqcj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kyoimvab.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3quxnzygu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yhrsefym.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gjdqqjcy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gfooockg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjbxiokx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkcuevm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjqevlc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqnqbpt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hemvgcdi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ejauyzzn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tdzbdpkn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jdctwrox.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3oztjntzo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3eyriqqfm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3kvubzvni.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vuhecyuq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vhyogtss.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vsmuikmn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vwwumvqp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ihfaztwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euuaxrlf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3miihmorl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhvnnecz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3pgdaqxil.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ntetneno.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ldwojkxf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kppwmcto.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jsyoqlan.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xyxjwvlp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3cxnvlwje.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wwryilmr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gkortqdb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3acwglshg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pmmuexaa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcdxdbgq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ikrdkbex.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ccmihlur.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xufpknac.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bjozamgq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zuayodqp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bzadaunc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3twlbbact.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qjjttdxk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgthgaat.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jewavuug.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cevtynzs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uohwehqq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gbwsbdxl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3pmowaxgg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nfvensym.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3frmveniq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ggibevci.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wlblfdyb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofookijt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bealxikk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hfocjett.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ryotboii.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mzjxsgfu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqmbdefs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lwfwfwif.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bqlvqckh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xqydwlzf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvycsdmu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftoqsibz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mexhpcpi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhveqqt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3frfnxiun.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3effloiub.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3dtwmagmq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3srsdxhux.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yopobezz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohcnhdaw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgzlsfza.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lxwhefjc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mtlupauc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fzuxzlwj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3negvovhm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dpvdgmer.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3stjuvhja.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfhtgavc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dlcivodv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ahooniwb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gtjrskmy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3iukwgykb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pxvkhowb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kwmpyhkf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hsxovnzg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3etfwiehh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tynjwshg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rknhaucb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kscwogho.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ccuqttpt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fcbifiqg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xurqbsrh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lxmujdtq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zgvrpyer.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3girniufk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3romibawr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3saazfipp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3szrwykrt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrnuaqht.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hhzbusez.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqfbwebx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3csfievlm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3uvbzwzai.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3orqkvayh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rauoujyq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jrmupskm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hsitlepz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqwrkzjy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfblcyls.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vvnpaojl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmbwasdz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tqobvhvo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lpojfkvm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3koimzlsp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpdujqnm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pphmbaae.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojpcwcun.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3iraxrkbq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjdkze.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ffnlabvq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zsoweipx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rhiszoad.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hegsfgkt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3coclpigu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ybgtgpeo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tcadmcez.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pifonflh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zxmxipjy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3pvbkyefv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3twtbefab.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jecaeeoi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3idigcvcu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gynxbmge.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hiebhatt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wedzmbsh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3occujqdb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3irhuinxo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yxfcjyla.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dhmmbrcg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dztobppo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wxzxaflm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzflwein.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tjsvcnbh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywzkpady.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3dbigktuv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gweipcxm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfomelx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ckltgnkr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3voktdqmm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3wmhjgbku.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rzqbgluy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jgqndqdb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3usolmozg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rryhmroh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mnzartjo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zcwfpcjp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hlejrsbh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ccuzxurs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hvzpvjej.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zegtixjl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hzjifcpy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mfyytpcg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dpmutkif.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hvwaalva.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nzyjaeop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlszausn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qnhowtqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vptlyahq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmgjtqzd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3btazlgyc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xvwqoyrb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcmocqvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciztccdp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgwcdrce.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fpyfixip.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3efogmorv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tthplrgs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ashjlhqr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kxotadyl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbfeqcyb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sblnajti.html


<!-- 参考信息 -->