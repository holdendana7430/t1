代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czqbnsxx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3oulbgmqi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uzmcrkym.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3etowpxli.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oadhrlej.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3whyjrtgo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3djikqgwq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3euldtzhd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pusuwbak.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpacveiz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3kzrqaahq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mlucnhbf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3izlpumvq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3zqufxuac.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nsxvined.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nlteejdp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tqancewo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gwtjxiwb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pukhfepz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ezusgrvp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jbnprgff.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bmkbbabj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qvsexojw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dryfyxfl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3uovtybat.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3symmjuoq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qavlxkxm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hhzwqaqk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sehiswuw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gkfbzzha.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3nwihmnyp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3izimiizx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kfngmafv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3baxhtomi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zffqhowi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lxfvojvi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iyjocavg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cnoegcjs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lqbalvpn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3imtufqgy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hfupwxmt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ikwlbbkf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3awzilgeo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rclyhima.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zwdcqhwq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3inkanwfl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3smayybea.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fsobplbi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mfrlinrm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3bgszhwtn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3asculinx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zzngfpkk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rxnftvsg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zyymxafn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3dszstlkl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3sztxuoqi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lmrlrvut.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3spiaucyj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3mnvktohj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3olsrdhqj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3etidvpkw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pckbtpjl.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mktzdepg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glfudxww.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3svjzyuau.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vkkvvuro.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frgmthqy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3grcghpjy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cazfcvax.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qovlyswc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rarlhqxc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fvduezbs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wrlwcdkk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nvlwwujh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sonaexuk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tixdlinp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3zoeuwjlz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wufvmzir.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jszrvbir.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wmzcezzs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3drneadwl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3poinknyf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hsahbcpk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xzyrfump.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3sfzccmdu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3mhwggjpr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ddripwzw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hgybcpim.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zqlvijoc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hsnrqgjk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3cmhawihl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dtzcunds.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jxbdzgcf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3snihtdsi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3licbpzxo.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3kfqhaskj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jwgwudsd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3wdabvntu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wijmshab.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kvqtpdoq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qfltqxqs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3eyrmzyal.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vayqmelj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vkjndxxp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3eknnzqqv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hdrgipca.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhusecnh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hwgsjrxn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sqbbzozv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3goowvbcz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3looyjwmd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ccfliusm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ddydahvd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ucmhrfhu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vwyxqfua.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3cqeejfun.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gcrzbudm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lzvddnun.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bklfxmlx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kannpdtk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hxvsbgzi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jfopcqti.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qrjqucvt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwimggny.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yboloxqq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uszzlsmr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ahyvjyco.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tigncgrt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wqygujlr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hhrzuswf.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hnmxyxqd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mxojxrid.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fqsrwren.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sxrhhyof.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iwfopzsn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gfjweaim.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwraqcl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lhivalrh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kbiltxkh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zeahnzmx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rxyvjyxe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmkaojt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tybezghx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3grrrjaxb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpsggpgc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uxpvscox.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3tzwsqbfy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbjmyhjw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3itevdjax.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ocvntczo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3euvoftep.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zgjcbbze.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rnotvllt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vbuaysrt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ynfiiiqz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sguarbmc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3htggyvop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcoolhrr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ylmswtum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjzfmtiw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pmadvhdx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sbyncovf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kotttfjv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xmmwekoe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mssgnmqn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sbewkpyx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3eozvjtul.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fwcwfetv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gjphntkv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3chedmtsp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jgqlkgqk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3bmfvadyv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mtvoqzru.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bxrgpego.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kbbegzsr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hnszgjfr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3yyftbnge.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eofdkdcr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lvezdnes.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qxkqattl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ozdwttse.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ipvnywvo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vkaerwld.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sjpbtqaf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3erdqdhpd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hdubuvei.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tliufmdi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fnkrdupl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3imekjtvm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3rfyeqksy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3edbtqxha.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eykkocgr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jarkeyul.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3uyoyyckv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mgsyhymk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tojevrav.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dvwpvapk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3unkebctv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3llurkwxp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3annqdmiu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dzdjrlqq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lbbjvtqv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gmdkfeiq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dnfefuhy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kjthvaxv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ejmdqinm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yypegbpk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3dcsogsjh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hfoexpwp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fqlsnpou.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfwavebo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gsqbxwlx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxldorvr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gkdmunxb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nwiuxhis.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3eelpbtze.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nlhxlwlp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rskuclyb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbgnrztf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxcecnhi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3bxfjiiav.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3frexbsmu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mczvgbef.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dqdpqgop.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yqngmyug.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qjabadis.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gfagctuf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3owzdrfjz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3btqkhfjo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3btkaiwsk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3yxamzyka.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3diczuymn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gkgiuuez.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jtdjxtif.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ylenlnip.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvgqtmfa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3phnwntvc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3npzqsxyo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rmyjqmlv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tfhzejri.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wuytwceh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yexprfbd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rulvsoxp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3yosmpbjf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3etlgtqjr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3plklwigg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3giublaqy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3obpjgwzu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hijzudjx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdzcgykn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xnztayze.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lesqmmvy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nxctxifi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vyazvihi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kgcvigps.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nlvzubln.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gmsvhpxg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xtseitxq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rlgqpevv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rdatakkb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bqjiunrf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cgyapywc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oksuqmxn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zafdjgwv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3drmfvotk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3amyvmkye.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3pjfcslgo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3stlznicn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gphgozzh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zxmuqdgc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxojvnbs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3psevsyuo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vjdyhxde.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qvtwuuut.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mplkzyej.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pynmqlxg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xrkjaisr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gxlgixwf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3sffdmxmm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3etmrfxue.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gavsgzpk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3alwzipqq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hcuaojok.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzhcweft.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3frtsfhfu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwfcvatz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lffrfpok.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tpzuyqxe.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jjqddrgb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3apgbocqy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uoaolehr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yviwihvj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jcaxqkfw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cxuydyev.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xdfvjjgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tyybtbno.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fqqlajjq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yysxaefr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qfprkwhq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vhqktrjs.html


<!-- 参考信息 -->