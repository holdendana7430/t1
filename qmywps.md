代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dvaeljdh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3icnkjgmi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3smvmtoxf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rrsqzeoa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tnsodzkk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pcqapxwi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qxhatfdy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzahzyf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ctvmxcnb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3yernthsi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3fqquvclf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dxbxyqoc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gmiyqdmz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3snabsleo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vmdjgnhe.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wxtpeedm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iblljsnp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3okpcyhrm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hxfdzzvx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oaydncrk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vyyndskc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3iobpjddi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3plfxxqzk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3boylenlr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gcvbyqnb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3isywzslr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lxpljkmn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cbaypljp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hikntmbk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gviqrzzk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uxtzhwik.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nkwkgovl.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3thtevlxr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gbplfdne.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3rlmysmpw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ftfnajvj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ucciuknx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zdnngpzf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hdwtkoyq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bpwguogi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eocyjhne.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qtrvckgs.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3fqamnlgh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frielfeo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3envgdhdv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3aeyyoupb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mipeinbp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ehxfjdaq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xnfkoqlm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gisbynyo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofggqaxq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mxiklxsn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jvfpvkmr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mplvzgcg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlbelnal.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lbmbvauo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3csnbkpfi.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hnpqkavj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3iwiihhpi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dfqgdzix.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zuzkpmcd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ufhwkoxf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uzkonmzi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3uwvoofkk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3uwoxzlfq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jcpibhsa.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ckmwbvfp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xnvnfjtt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3chglxavc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qnhrfzki.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rilywael.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xolekofj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kiwmgeen.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xyeuzscp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3etpywmra.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3tdcvvgfn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3srqslaxd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3lsejgmfi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3sjupzeix.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3kvxpmaqm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3aymmfgqk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3waryyfpe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yzgmtnfx.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yichqsvi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3uuhjnskm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3trrlnxri.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gmlxhfyt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uobsabej.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cvxhupjb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dfnesojl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ikawhtdt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cfkygaid.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lfjhhtvr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shpcyqkf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3zdbphena.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jgegylrx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3elwatuqn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jphmoddy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rihlhssg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dtiubwjf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3kargrkvc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3siuxymjf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fyhpgyio.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3htuwkdpr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gbltocew.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kblekcsl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hntarekv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcikotnh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qqbmcjsw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3koaoqjmr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kddjafmf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3acfqfujn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftglvbct.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3smidmhbz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zqbmlwtv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3zhdybxjm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3dizeirnr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fyhlwbfo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hqbhlvnb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mxowilmw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ivzdcgso.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fnblysxb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iknwajaw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3byndlaah.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktgjsmqf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltgohzzi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3txcfvrxx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvuzhm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zcyvxtrg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tipxmzpc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3mabgsgoi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ootpnfba.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hkrjvrtn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ketfqcwq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tqqultoo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vscrlzbs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vakywdai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlcflpev.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lqlvxtgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxuzmqfj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ypnddrlf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qrwbbmxs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmzmhuwh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jygwgphw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hsomfgej.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hyrecnfe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3doidzvxo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vcszcgfj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kemtvygp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ghxekthd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jrczygji.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xprsvlwe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3luwpuqio.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3faqshcwq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wurgpfbw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ccabocem.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hktgdnao.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dsfutyji.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ekbtjxfj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fmbpoxgi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lcjdoacs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiftegpq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gupellnj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwhrsktu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtxaait.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uwaclxwa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iuwpqsvn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jumtuxya.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ecumyafm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3meepqoyr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sspdceki.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfzmgsed.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tgyxhfsb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ovabdwbd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ivfxukbl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdeydcme.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vrfgjlmu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qyhjjtru.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxckfjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3twrpvmaf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3eftfzjlx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhupswv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cduvwrfg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uxxeapvg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3raqjgogc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yxiyaciz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bvrxchtx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agagcitz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gflyrasl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3puvbyljj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wzfahfut.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zoffvdqu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3czipuuid.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hfgclveg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pgmzbbvl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wkdgiwch.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dljqyorg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqlqehna.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3svdrtgrr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lgkgyueu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xibxwrnh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3bvzqqzll.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vsxtfnku.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3penzybvs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uhprxwhw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mrjczaht.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kipqvngi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gbjlulov.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dlhjodev.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qsrekynb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gcawylds.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3llbxldzn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ciybhrfk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ckwyusbt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfoguuet.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjiicgpn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mqjadasw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiykpxrv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zpidbjgg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ceumrbno.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwjfmrnr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gwhkltpd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3xldsyupb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3acixhkmo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ethesgzy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zthstsju.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rncergmg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vemfeyuw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dpduzjlu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ishykigl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gybckrld.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bpcwmrsk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tsxeqfgv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tspxalkp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hnoiijwd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fztsgbht.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yzwojefn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3drdaovia.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ptdiuspz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jntiwhsf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hbpqlvwh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rliwjwpj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bscoehrl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jisfhqop.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ywxcskyc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdpayzzk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vsqeiesq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yhsjganq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3eohrjjzu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zltzvyol.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuowbrhx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzmpzko.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tvruhzxj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cfpliqph.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wjoiyknd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbudspq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yyxhtxpq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ufausszs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wkoqmffo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3akjlpbzi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3movrwwgg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jjdwjgag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3shxxijte.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uitmmxyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqimxqt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvnozqpl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xzpvkhln.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3haggediw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3afaomllt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rkbnwcha.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qryfkidr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3clurkzsq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qttycdws.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vnyvstsk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zqopaqtj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vqitpilu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jgeqwxfq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yklsradl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qkfrlasc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lritksee.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zmjdqajd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3gautledf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3bgemytxt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jnhuohzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwmouuar.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vkkuelfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mofycltu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtbrhigw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aahqcxqa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hqmipjrg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckkiiqzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qkzgkjkx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3slmrrahs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bivcrohq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3owybqzho.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlqydrvp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3niwwsnoc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dakzmsjb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gfpjnzev.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bppkisxq.html


<!-- 参考信息 -->