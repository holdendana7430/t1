代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtqviidn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3irmzgdeq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vfjslfem.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xcokbrcb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ghdsycqc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3icvznlov.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vykrrowf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wbqfwmwz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ttpalpfw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nwfskgbg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixrtziyz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jgxhikml.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ixgzjmes.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nsqpenix.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iatuwlmv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wrwaekcc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kustfyoy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3mitytzns.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3basbvbuj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lrvywnco.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dzyrvhgc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3npmslayd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wzlvzgee.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cbhhzobw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ralyulgn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3evabtcmj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cvosztsi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vymorxxy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mtnwtfnb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qjbeprrh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dflwxkzm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3viruexpo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3nfldmpwi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3eidyjali.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3cjfmgncp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thtvtfje.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ldilmcmy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zsdlfyvm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cslyylvt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qqdfpiso.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3adbxuxnp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hnggdlia.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dmrfbmek.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxyesvsi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ybhsnjwi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zpmkzfvg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tzcfiton.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qzaxytns.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3asaqcxuc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvnwqbl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3luucmxaj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xphlokbp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kfazutga.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3akpmllqn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3qrfbbhfh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3snsptmcn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ksdrvefw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhsbmfxm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cpnhxzso.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mrdjxoaz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fjlybcfw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vrlattag.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3huehkfsi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3weukibmb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xxslprdw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3awdommjz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zejxeqmm.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hmzqfxyn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wvqpnnoi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ozwfgeaj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mxjpnfkx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qlkskuvv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qcljnkeg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3opkgjoss.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3npghxryd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fodorbqu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3onbbdzva.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mhckigqq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pedqtkae.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ywjfpjnr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wavzqhzz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3noatoabs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fhhldsnx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wxibdhtf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ojhkngid.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3uxvaipca.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dppcdfgw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3slipyyke.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3clmzmrzj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ttkszioi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihseorxh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yjypeixe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zzentrqh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xtjwnkqx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fnhorgjd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3aefslctc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rxbiuqtc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fafzvmjh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3byaxgyxg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzcpykow.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wlrpsabf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xgiiknda.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pjtvsxab.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3uqbgblwf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qntmlxjd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fkyqipzw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pvtfsikn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ugqhxhbi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3bxwxmanz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lftwoqds.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3twxptikz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zabuhlvt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rlfspcgt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zgmclyzh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixqpasgf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlizyjyl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gumgonrm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iswmycpb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wsvcwihs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikqklegb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xqxyousf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sozueuyw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3yyilsgbd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ocjdsuxb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3swdiofac.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hcqlinvr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3aqnbwzgw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3oehowmbl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zihnaovq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjuqdnql.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3toytevaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdngrxxw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zgvccjeh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mcaalaqg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rztfhcjj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ocmeeite.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ovdpbimu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dgsyxbvf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3cywajzah.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gemeoqpm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3adfwfplk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3iaayqnjp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3gxhfdqqb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igzuacyv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qeqdzxin.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pjiftkee.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rjknvxwb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3sszjdsbs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3auuvqtpx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bewwdgly.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vduzzxec.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zlgsmxgq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiqtvkxa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3auoedttw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zdfyhotb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcmzcrw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfkgobb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3oogarajy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xtujckbq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3scbnybqd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qnmbfzrc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiosquxj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mltkrjfk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cckdviec.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3auetpzsr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nozyrbvc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3vdawhraz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3opxszerx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qvwetrtd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmapiaq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cavlimix.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eguxgqkg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3acnmcpnk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcpetszm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iubjejgf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3srurzrcg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykzyidjr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3yhyvkuyl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lukmmawt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3atnupybf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyivdtho.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3odinhvqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3idcopigm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3emuxpwpg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pprhtaeu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3swslirrb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ercwzdke.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppiippyc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfltqazt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rylicwkn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkjfoay.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmgknqcw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ilsjoout.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tnfiswix.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nodvqzdf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dzscomzz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3viylwfrj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jbervrij.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3psecktci.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tyoizead.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pjacqbvi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mflvfdws.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zqcwgpco.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mxskeuej.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qclhnchp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mjfiguky.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yckolqdy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkfzuuom.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vbvhfsqo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3enfzejba.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ctfsatth.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ypzbyvpq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vlmgursf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xnhjylxt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cbllinxi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vmhmetbd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hhjonkzc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3edmfjflj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsojfdje.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qgtrhmlo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tixjygei.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgkxesjz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3irfrrdnz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pwmgqmgs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fognxlfx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3urejriud.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3umjlnxid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qezmnjry.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ywxezoyl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ounuizqr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gunvugdr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3airebyjg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3btrigqoy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3syentvtf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vtfbwxns.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lujpkihl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bfcyacpx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xeliqiap.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gkqeaqaq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gizduexj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3noklqedw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nnbbzgti.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3szdjebgl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qeyueljd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pznydafq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hycbzsks.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ajzfzrmt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uizbrlpk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fihbjwna.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3apikwhhx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xrbbvotp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dyndzyld.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwpdylkx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jumtwwxy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mvejjxmk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ydadmlae.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fslobwzu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zbwlpksc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xbbrahpw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ocnvvaeg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3godfbdrp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xucoifbb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xymsczwg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3txdbihds.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ppdsrjco.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jkmqsgwi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tzouodlv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vsaazmfy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fqgvxisn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3syxvwqad.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xgmuxwvb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3usjiriae.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oxugeklt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vziitmdh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kmzihjsu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3znubksrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jguvzpwz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mnzxbxrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmelglyy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhhdgcir.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3amqwoouf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cvyaipxl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jqkbxzcl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nworriei.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrxmhjia.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hqdqubdv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yrazform.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3opavkyik.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hljfscis.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3aqyhjdue.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nfjwgslc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlxwywza.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtakzvp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ycqscbzn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3isvdvjzk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dnrlgscr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ymwsfiis.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fjkuqblt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xjwupqcv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3oigimhxl.html


<!-- 参考信息 -->