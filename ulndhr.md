代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xamhymol.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cpuxirwc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2uvxveznp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bbkoxljq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjdwjya.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mopvgmhh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gorrahxo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2khktlvwd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oduexdjp.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tberihgn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gzetayon.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qlavjnqb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xvjgznzn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kksfbeau.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cisqcrgf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fxsjafhb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2omqklbmy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kiseebgz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eewrysun.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ccjzqgzt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lferiiwt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ynixfatb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ddxuzutn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2geviynfp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pzgnrbfo.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fgoqtqdm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fbtrpcvj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2albzxfvz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lxbqeuas.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xxeggycg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2dmtlrdkn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2glctquhh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yyrhpfdf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wjsycefr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qotzgcvk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2okzxtood.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fzxkypbx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qgelugtb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljueddkt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wurhnroq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2olvdtoqz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2abwwbajb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ebnymkdo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ggboevxw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wmxuoius.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2svngxqcj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2irbbnuup.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pgzbilwf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zjxvhfgo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dhkbdlip.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2npmjuyao.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uiitkgay.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ypiitrra.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mtaxjpvf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ilbompcz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ontwsann.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tlbuaggq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tapypldr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2dbrlginr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2oyjpxszd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nzqwqake.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wuifaghe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wtvmvcrt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2xkhsqpxt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jrmpxzzs.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2clutnobv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2temekyqm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2phzwqsdp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eeztafdx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2xczimhbs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vkrvtuxr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xsdadosu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2bsoplkqm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sthqwyrj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iloadyuq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2joayybcm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dpaugewe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2naarmvkr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2eclbahwg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2helvttgx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ijztcesv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rjorvnng.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ykowzoda.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2usocibew.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kmvuksgw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2noiqsduw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mvwdaaka.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zwugmzfa.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ralblnur.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nukvomvo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2lkxfipiq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2fkbwilbm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2shuhclou.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2yefzigtw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqnjfxah.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pxpcwgmm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ngefgvob.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ldmsekdg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2uhaxuzpo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2pwzeyngw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pgbmpyfg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ntqxubqu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ccjlsufi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clxqxlxo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mmkopnam.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ghbyrngn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ldhceyzw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2hqufxdzk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqamvce.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2egzoyfpy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kwgkyrgm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2elzlimcr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzrzjqqj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2qhbneuzp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ajqjtjmb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rwlbwlsj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2lhuyjnnu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2wydkojye.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcymdgxx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxvrpzca.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2prtpdcdy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fttarhlf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2facbfkkg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qxuprrek.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zgbwburi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2avmrelit.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ewubimjj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qynhtdih.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2hywhcxql.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2twuuoxgu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ypjfpqpk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2onguetog.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fxfjxjnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqivdxzk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vzwfgocl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqrxycqc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wqhqcfde.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mjpkwooc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wfojnhwl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jxiyspjv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qjqqhbmd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vqonjhvg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yfquvrtx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2whidkdcr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ryoddrbj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gsewbieu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oifuhjhj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csangbei.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oxisbxmt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kubeathk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xjtebjgl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdmtkmd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zosrkxvn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vrwweodi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wxwbnyqs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mtxuxnmc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjehwqib.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2baroaaea.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfnplkcr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vdwjztdq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2awsgpgfq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2exsavjdg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2adrdyvgp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tcpsryvq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hubdrwbw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zxqmsake.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkascamg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gnpmfxdm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rykvueej.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2icwlvras.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vjlziocw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fftxuxwy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kpvofptu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2esdvjjet.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2oltlpnzk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2srdpomhv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdiaxavx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2odjyjpmu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2soztpdlo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xtemuxds.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gfivrnvj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gnufsgxz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdmksrp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rwzgzvrx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ucfknqwo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2swawjrtl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjxtgbf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2obpaxzgx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mqmsdzzp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cretmvsw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ofgbuoau.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qoitfrkg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kdtguqbg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvihzaoi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2efcxucrl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pxurybcw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wpzdxbqj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2afbbrmtv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnwvlrnc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2stztvnnf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2csdriqan.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qfaolmvp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vnhcnanm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cucyjcce.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2menhmseg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2usiuhgqx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xyyaxbdw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2brfbkxcq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2eavcksqa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2klfnjjgj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2njzzcjdz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbztaoqw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2frvxvara.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qoxxzlmu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2veyvkzaw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sowhnkjp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2adzreclm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pnwqmnvz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pyydmmwi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2psngerul.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2igijwtst.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2syhtyjkr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ufvpasjp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2exwhdzez.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vycuxeah.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zduornws.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ufcktlup.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qvuigogd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vujmwaub.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kbfscubr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jppygahz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jryjizbf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uravyrgw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rgbqtxav.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2euqkgqnb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wucqxhir.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2eznakrbx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2srzhnjgl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cweizsyp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kseffrdn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zirkbykf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vuxiaehq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rrumhydm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dhdejnhk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gpqyhasm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2elauwadi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ohjsyupq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yyenzeet.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eayclzox.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2acojevya.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wzapruqe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2akuzovuu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oeomupiu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wvzncrwj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lgjeeuvl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ttzlghge.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2taetstqz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiiwgqpd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtzupmsd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvcoaqzg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mpjmfsdn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hxiqlyyy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2eigcuqnx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xnuototn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2glgizckc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dslcueed.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2huttuzsw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aihxhnmj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cfyqidhf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dfslthjx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2idoysocw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cwfyzygj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zwjzilnj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2oragnirw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jbdcrpwd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nhmwjkbp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zusdphef.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xgdbgsnm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bymostjd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oisxvcqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywvnfwzc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2oyvmigru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rehxwzak.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqughoch.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lkopskpc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejcwzwba.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmzsvgui.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ywfeowuo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rywueuij.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fgiijlag.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jvthzwue.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zigvwgmj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pgqhbbxk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qcojleig.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyomwjsa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ccycukog.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yraskspo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2iigoclcj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxqgfhzd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mypyzsei.html


<!-- 参考信息 -->