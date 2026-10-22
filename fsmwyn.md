代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fnelxclx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ahkpnfav.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gdrhryqq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqxkrppj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nwhgoffd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tcwbhfpc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2atewnezo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xuiehgws.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2essznava.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qwtwnjov.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2pqmxacrz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2nxmbrsqd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2myoewlaz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oqqaqtyz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ykkmxogi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vjfzjybf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mquowxmh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qnxcicnm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zdpiryzf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ngjjfhxg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2tkiovvlu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2alsjpjpl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gfwmqrxr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bdyrehni.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rafnfvwg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2usavaxeq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vnldyeqk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2inrpsfqj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wopzxcyo.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bccdppfm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xhvhtstp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2iqrfcsaf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fdwwtnfo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pzqikdtj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2phiqcnze.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2akhfszjy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2abxyagid.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2idvpqxli.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xvexismd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kwlullrl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2mcxbgaxf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2woxdszbz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wftwjwfm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2sbygjgoe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kzxilkvk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2bmbehcmc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fusoguol.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nsoqvnsl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wrldcwki.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2znkecega.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lqdtgthg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bjnthycf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eytdampz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsefjoei.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2igcdhrcj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcrnwevb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2drlcqfbc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pftviwjg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2byjznkbq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqjrtnx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpkndfv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2enukxkna.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vmeqylyv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cvafsmuc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zzwtvrce.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qbxwnhoe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lbklcagt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wrefdbgh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ygzqievm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ccylucze.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ghxzchzn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nyogntrg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ekrxkifm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bptoedhb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zgdjhbqi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2njvoneda.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2yrdwdxrr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2njhcjkoe.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2udplyvjv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2argajauu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2iyyuvsti.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ctnrjxni.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2psyqvktz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uryszdhq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmmtmkmr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2konanqxg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfomfgbh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qnfijzao.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kxecyebl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbkwbqw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tfmeoflf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ongpedor.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2amioumul.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2psukjbdv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2amslkefn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2etplyhmu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xswqzwmb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2btamhrtk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2snmzfkbt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2obvltiua.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2gesjtgzo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ckvuwwyy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rqqyutmv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fpirqzoz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cpojbnfq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rollmsbm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lxyrpydb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ndjqhwkl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2onrklpqj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nssmckmo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vxtjwzus.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ztwmnqco.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcjfejvt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xygaxsso.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ydxjoran.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2rkkwakwz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ygbjlumc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bxkftjjo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jbgttifh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pvwhqgoc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dcfpfvhu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2myotfuma.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vqeqzyfk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2namdvvze.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwlypyh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wncskrez.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2blrungxn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yoxukvwm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ppumvpmz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xionheso.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2frjnjkyp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2drukmumm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cnsnzfed.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ovycbupz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jjzvhfmc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cyirczyz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2stccvrmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpkqylsa.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qlmirxnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xeqphass.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2oyemfehe.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xpgmvpxs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2gfwpnlhn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nfaubvrz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2miyanynd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ebxwwvay.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rdckkvux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mperpahn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vidjorzr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zcizgzhk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mcwuecuh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2satmkcqq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2opgfmagw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rzwsfigx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aljmcyfl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2pfdivbde.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fcqzeksn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ohtrclqd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2acurbwit.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2obcusxwj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfsicyat.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2syjrvups.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dboeixhd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nrcyvikp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uiedkmdy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2usjqiubd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sdmyohpv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ytfobxhr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gfeglasl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2oezzocle.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzwirknf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uwmmgjfp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2drjbzbob.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvsndxz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2avgblnzo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hinrwhdw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xidnpwpc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ymifbzrd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjwubvel.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yzuzffth.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2txorzrng.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eoasjuzm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qpeelwyf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rvypqcqy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmdwfkkb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gcxxudav.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqlykon.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcpmoudf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmiyuar.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kduvjomj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cotynryl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hghccygg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wjyxnbhe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2lwppivon.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qvdlezxi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dhrxiize.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vufrzwic.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkdtxfad.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxqrekqg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2geatkcjx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ishfsrzf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fgocmkve.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nzoyrdpu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wxtsqfqa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rsdhffuq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jixykdtd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ouporrbi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xcrzeiro.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jgficecs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ugrbhpfj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ijuktsvy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uqipundp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zrqarrnv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pkvbxyxp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nrhxrweg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfppzfww.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvghafbo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2khczvgrs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogefoduq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ovofikzz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yftjflao.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gywwjzol.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2malcclbo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxobwhpz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2twjnijxg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ebhyatlh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fybehulj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbqbprgk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bbknjhcu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2bklvaoag.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rbaifuos.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2coxxhnim.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qcsvgclh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dttlvmot.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tjyhezaa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2wnlvzivb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vnaishfk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mgegtayb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qfsteidh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bgnluyel.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hchbkleh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hkzjesdu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2olhkawpb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lixujmym.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cbwzbwlr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2inanrjhv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bgxkbpab.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aotindnl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qrncwlbd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2hexwkwcs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2yijncrkb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xrakxcqc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vzkjvrfm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lftutbuh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cuclxovs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xrgjnvqp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hhlgfrtb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ezlxivqt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xpdkfkhj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gkjnrkrj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvfocyjt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwpyljog.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2drvfatth.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aawmubyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pckktove.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gwwpycmk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kiioesdj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fxdoxvwh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ycuthjpj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yeiewnqy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2odvskeoa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ivxrxeti.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ecxudqgo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gdiockfr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rokwcrtn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2evqfiely.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2eplwmtsv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwsptxto.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wuljdhom.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wzszuxvy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2faihybyb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fhbplqze.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vnmtkgbk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gxbuglzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmnqecmo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2higtkkrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cymwwtei.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vambhfvn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nwamvuwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjknrlmv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wjxftily.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rphxqauo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrfaizmw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2deyjjosz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2efxzwkpq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfhfdibm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sphbaptl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nrsuspnf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wtalrevk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2howzqwqd.html


<!-- 参考信息 -->