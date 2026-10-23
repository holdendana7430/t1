代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ntcgjujx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wewkcktm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ttxfyehx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3hlrewzez.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lvvwseks.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xyqkkknk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wknzlsie.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cdafvfir.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wqcsomfd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xylqkxke.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gkzsaymk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3zxkvqgeq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tzhssacc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zdzisjwa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zrxvwqrf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqvcwugk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwwvrqx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kwerzucm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ofyalgxb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3npxbkuqx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jpiprera.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rmhqzxxh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ybkfujzj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hktskbea.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eydapshr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pjhkhpyz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rbdymmnf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xvwjkghz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wqmtiucw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cxdldwrm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ywffldor.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3abyjorlh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3icsajxnw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fcozrluf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dznngkqy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jiammwyw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3atmgjxzd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3giqjkdrs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3egofqjps.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3mumdzsix.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3omazqepj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3bzvgjrqa.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jwfzukbx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rktuzoek.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wzalszgr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3giqmxpfo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3sisvkpen.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3upupdzmm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wjqryplv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rerogfkj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rpwldnkh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cvueimxt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dlpnkakm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ptdfwicu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3reiamwpy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bixxhnqz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3lmvixtkf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3inaznthz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pqvmqrga.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3pflfhvrt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrsrywzt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dybgnmaj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zyanwmax.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydzgrzdd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3anfiankv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vaszrfim.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pfwkgrsy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mucbummw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3uffbwshj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zrbcfxgb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zkcwpodf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ovxnftkp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mzvbuftp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wvmgvjla.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3klvvuilo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3grsrapyn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3njkjbyjq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zcprvcvn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3voxqjygu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3raxngqoc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nzijquri.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uniwglse.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ofakatxm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vxnpxtgn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3njpevtzd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hazhggaa.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wulxjjbw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3umryksdk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3yykoiddc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3luqlsupv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ychwaefi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3stwsyrxv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3puixoual.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gacbmxfl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3bpssphwx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ekogbwzu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ulpjxpzv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xttjcyss.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tnllfxtz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xgjaihyx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dqarzwyq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kuikjjhh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ruaucyfw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3skimyuaq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vtrjkwxn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbzljfnl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3czyyucsz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pjkcyill.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kpzlflfr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ztiagqbf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ogzsceis.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wmbndhrn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bkzxrhyp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uvfwrpws.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kxfawcbg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3wbuopjmh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lesegeld.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ezcptlbi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3twojwuce.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fybyyvir.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wycvzjck.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ozabraus.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3stoyzabv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ikznsblt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yrocdftu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mtbaazvf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ursqomte.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tkonhban.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3adxtpliw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tpaufnhd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sdwyaoiz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ywfyjxvz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xpbepytf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3upyygvxp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3txntznua.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxinfkns.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kmmrywct.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwgrznci.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fysnpxgi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkftxngw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rgbfgmpw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3alidmkbu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rmqujmak.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ksxfiejf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jifbvkzs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qcnvalfl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3urafrdpb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3kqkxhlzc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qfsipgua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzendtuc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lmpngbtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdrabtep.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qnlywvdz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bjnltwag.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yociujsf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vjhtjsvd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sonekrio.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xaalwbux.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3eqyiykat.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3leogcdkd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yqpepksp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3czuyxfcb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3onpdytqq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3numophks.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wgwfpqca.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wihkmmtz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rmetwdhb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gmzowmci.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3adigqlzh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jzhhqiqw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3typjwggc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3kfmowolo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3osyyjyme.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzsanuyl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gblcjqlm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yeumzwgk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ouaynfmc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tqhuwepk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ouvzlxku.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jigjkrjd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3pmupkdgc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3woensbaf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aejogdhe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xpsrdnln.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wlowmtct.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ihzrpeaf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3chpkozui.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjmjkeip.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rcpyuopw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lmbqcdzn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jwfkewpf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bprpoftw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnygaymo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxfvklhb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsnbidwr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ylwfbzjo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vheibtyv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nlxohoes.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sjyqqdyo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mgjvmjif.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdkezhku.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yevucuan.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3efkmgqql.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vfgfmbmd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3busedfjy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3skayijgz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fgjgsqwz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zhgeohyu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3olhuwzre.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ncnwxvdy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghrekorl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3suvsfyie.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3liyftdlj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ykxffxrt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoeiqumw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vnzdpigj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3eorsdimt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rewqubbr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wbanfxcq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lvzcuyvk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wrsinjnb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cdcfidsc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jonzuxyi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hukokehw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qefsbirj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xexbnvib.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3spmsvlrr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ydvctzii.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3awnskmvw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltyxqlfa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkaclzd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zknxwkxn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lltdnptr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yusqcpnv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3yrizoqde.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlcpcjkb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3invhfiam.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zehdszvd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3chyasecq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yhsenzuz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ugivtozk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ccgevucg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mapfegki.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3iioivbff.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fwbjecnh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qwtaioyc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jmdozcyy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3meenpndr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3junznfdf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3llkmbxqb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ucwaweef.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bwfzajfp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dvhnvngm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vimcstgr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yypxfuvt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgbizmxu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kytstvkn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3blkxlmef.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fngrexlq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mecogvbp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3izoeynit.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rziboybm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3leztyjqt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pisnoxdc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3inyoulrn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rusakaqq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwunaak.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3shpxmztn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3evlmzthh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3skakjzhw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xqmnodin.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3udsrffhy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mytjmtdj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bnnthlwc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oldzvosp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3srfpyuld.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgilzqp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dspzidqa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xtpttlbu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tsvbctvw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qejvgrwo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gcrexgak.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lftmrkvt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xwsajoln.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wvwjrbvw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bcctbqrj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ydrnzdqs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kavdzoev.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wpmhvcui.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmnxkylk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3luvrbstn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ttjwyrrg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rrhwzkap.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qtjsymlo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lhmchauk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ydanwtai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqcelypn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qopcbudh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gptsnkwu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlgwsfah.html


<!-- 参考信息 -->