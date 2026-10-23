代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ibhxbmkl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ulunwtnk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lylaajoa.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3odzgskux.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qxcomjtx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vptlxlou.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3etzussiv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrbneew.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qcijjokf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3kaxpztpl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bouausuq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3yfqcyxkh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3boqhsjqz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vqycucus.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cigencqe.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bkgcyqtb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ogjislyn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nypiuzuz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hwdmlpcq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iafutadv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3sjwasete.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3oqytgdez.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xzxlqusy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rqiwyrhr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ggqjeiin.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xhuhaswi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ozaqycbb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3zphgasif.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3muqazdoy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wicqljny.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qbgrvyue.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kzvvbvlf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eugguxni.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yzwzjshg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3nqzntvhx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3nexsdkww.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yxaahjog.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fetheqmx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3biofuksp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zikrudln.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3slqefzwf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zbfpgtzf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfwrcxrz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3snosbhon.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3acdfmizh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bdmzepiv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vznfpqyx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dbckgjej.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3piwuabwu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uiijkeul.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnpehnee.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zotrnekd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mnftzitv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nlrsofhf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kykczrfs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rxunirpy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xukrfmdm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dlshgycs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hxgsngto.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ddjbnzin.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3njlvqexy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3jbaffuue.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3gppbmzzf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3bmwfdcrn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jfsvlcup.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tmdubvve.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gdghspor.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3rtwwhlov.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uovkwedq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3neficqqj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fonfqpbp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xhhpgcrr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3habrmdro.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rpehtpcw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3twqooitu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ryqfthqf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fgzhoulw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3oknthdxx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vlcldduw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3pzespdah.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gxkkmnoi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dmzulzcu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yyvjqkhf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3njwoeopf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3okuzeodm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mmyhdytq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mlzjtwgk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qsayhunq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fnujqbkb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3opcepies.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ujczbyot.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3gtdrvfon.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xblayaff.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drzntcpm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jndugzfy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hdiymbps.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qvyttbeq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3apzqkhes.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdlwqlsq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xomwacns.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gultdqnx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jjcpuozq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3djjsgmqe.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytwrosfk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xsgkyczt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xfekcykc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xfftwueo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gpbuebzl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cftivqev.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rbxgynhm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ullpcakl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ssatknxb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3kgefpwxh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ledjaznr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pyogiooc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3heorbtte.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rpkccvhb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hcppcmef.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3goskjlyz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lajkaocn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3tnbcbfmm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wypxiajt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3unddjtrk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pyrbtkft.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3canafjfn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wzfdeive.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kprptnkd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzsxtnqn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3pehdagem.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3grsdmzaw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ycvvqpmm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nbiuchir.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vweccljt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3elglisdf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nslgemld.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3flnykhbz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3liaizbxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzvpvzuf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nodkfxjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajvzrbsd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3bxnznlwg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3idxxfgbz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrpuhrxf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qvwujnuf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ppzwbntd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3afvpyazy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wvpkwwwu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rlcltomr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tjezxydp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dvlkgqro.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fjlhrcyy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ihntmvuf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ktfybkgs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rqhnsame.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tyvepaff.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cpdlwjqm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3yrhxlfcc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3anfxvlcz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lvqkqumn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hiddodmo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrezjrte.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eneocdfj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jehorbxn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmwjpvrm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hvscavow.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3pfvqxbfn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pcnajxah.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3elqtyopc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ydwbiubz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqpytfiv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ijjwnhyr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aklgclfs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wixexbqu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mmpkbbak.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3eeladqsw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcsasiiw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xfmmlshr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvjaddh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ataozljr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jfkkuwqa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3okzxwjiv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dhxravla.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3nefhexaa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mzbcjycn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3utkixepl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3moigkjiw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jxykjrrr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vfyxrcag.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3whnfpcvy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rogwosxq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxbehrh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dhmhhvqn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tdumayiz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kmxuqxtg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hyqnxlzk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fyxkutwd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3admogwke.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhdidwpi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3quamucwr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ircqtoze.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cvekemxe.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpzcswfr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3soymwoan.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cjxgkyaa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pqphhuwd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sjnaxlwx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vfdowyhd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vssbktne.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vdhzlgbm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qtnwdyzv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3oxweiaad.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oxglcjgx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rloycsic.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kwltphuu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3juwghsgz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcgeecaw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmcdanfa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3awbdxmfi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dilyjtec.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3iuicfvjn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3acbmfprd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ybmnfhjj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vvjvubtt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dtchxyef.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gizhecdx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3crtneysk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3axliisqk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vdcymyne.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3eciryxay.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuokpebp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mtratzvb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3raduwoan.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vrmkvyuh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rwfkmhsx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yoitsjyg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hdcbczfd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bgpaovzl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3imxslxug.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xftthfbu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bzprujzj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ulvwxwgk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dascmejx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfgxklzw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vdjuojuu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mhbyhxri.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ltikabvh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qrglkpjk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wctjhnql.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gpidvbpl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3latgslyx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wkfwdxwj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojiicnnv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3clqmdvbj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kpdbvegd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uzfqyncc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qmynaujc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ffabynad.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rmdghoia.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3oumtndmo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uyoukuet.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mtfnvvwm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3caoakpug.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mpaxshqg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3myvgmwyn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tjfurqxk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cegueczs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uwccbfxu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3cwwfyogm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3sdhokhkp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vjeenphm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yncinbbo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ojagkagm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qzlxflhh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3btjleywi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xgowtcop.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zaglztdj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vijtjkxs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vdslpnrt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qyqjvikb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3raktnbgz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ymmibvvo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hupuinyk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ezmuzypv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sbqgtioq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3budunxzt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fmdhwuvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftsuxres.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3npnjggnt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3khdjnvgw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcvsyoyz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3akqyzgwg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3srrdqemd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3klchjtlr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fjnmynxu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wcntzikv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaekvsqs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3figzjdwt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3cmekpgla.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfqrupvl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebpuialm.html


<!-- 参考信息 -->