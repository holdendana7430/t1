代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uxkznoyj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2twuezuud.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jfikdsjg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bdmyrqab.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vbjrmzng.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rquqegxg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bifniflj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dzsrfnmz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2phpeqsdm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xvqckkvz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zjkzvpkk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2foiwwhcb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cnuhwhkd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2blkrapvc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fiuvnvco.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zswokmrg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bnirwgyr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wkaxjkpr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fhgdkfzg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tlfvfezi.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nqvfharl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jjktakuz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ncyzbfdl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nvsalabh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xdzntczb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cwuhrsse.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dzgfrdmb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kuuyhbil.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xqdrlwvy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lplwigmh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ldpsbclz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2tfdmbtlf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sxwknmpe.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2caiukkbm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lfecwkrb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2spjxsqld.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ylircphh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gyuzyidl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jlmcmlau.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlfjkbi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2osyosfuh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2szxszrir.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ilsqczwj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2cdaddfac.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cxrqismf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yfonsmtw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2vqtqdxbu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urcfayie.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kkzbzyam.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pccxlivx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdaokqjf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2agsmsdfx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2etpgpsnv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ysanwpqd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2steaaccb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wddcxbte.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ammcgdtk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nwtanboz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2imugtlom.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pmzhdtpp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2iavtkunj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2chefbibd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wmcgbqoc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lszeqiac.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cjuatbpt.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2fndiftam.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zfseauui.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bstbmgip.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2vottqdet.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfwcsupn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2enjbuuad.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2hdjzabci.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xrvlksgq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mxbgqboh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hjwtsnoq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eabnaemo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2odtrqjee.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2huqblamx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fznhbmcl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2spjzykpb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uhljqfkf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hmaazxqs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2exempusm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2twmezenf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2fmfabpsk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qvjtcznq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dcmmbkpr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2nomlqybq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnwghvrf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tubitunz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hjsndeau.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvvijak.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pbvabdwr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zelyagyq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ojzrnbei.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mdscemal.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qsmwhfzp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xizckylb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mvhtdqcs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zkpbwkfz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkhwcaxq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2pkiycpqc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkjiemr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uwfbaric.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2aoutxenq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dfelpzbq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2iujqgnas.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouumglxn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lhqgqnuu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qwjehnas.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bskfmmyb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zhpmqohe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ncxrijmh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zjzukkxl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2pnqnsvey.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gvmfahxa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qlcttbfw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yfdpvpup.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pdcsgkdv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cgaojpix.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zousmxpb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2aflolutl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qvotohhj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cetofnte.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2apirvgzq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukeijplj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jzkdyhly.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrhpmxx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rleybnue.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ghlqbhdk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qdkiydpt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mpftjvuy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2icubhddn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ujmjkgjd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nxoovdur.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2aczrekjy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gxaowtfn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eglaieko.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2paxvbdzo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2kgxefvoy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2niywikrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jboxpxfu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hfaztcol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kujcyqtj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zeryjlun.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gpaxkdgu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2urrzaofr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yvhrefxu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hctbtvbf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ifvznhsd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2yzucyhul.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2outevoex.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xgbfyuuk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2afpzoerb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2harvwvae.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gftezsyj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mjqpdscn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2awmdjdkc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lttryxac.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wfhcfuog.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lavhsnen.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yzggmtrd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dydsqvzj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ffflaccc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smqyplgn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tgvjpjnm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyqkukhk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2trffioul.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2onfellcy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2etnowhgz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hkvvisdi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nuwfqptn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lwoqjovs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2wtajfuzz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpcqnzm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgtopdju.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbbrrpor.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bjpjiqcy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fcfqccwb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gehsdard.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ocbbqiig.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wmbakhvl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhqidew.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2btgoweyg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zfsnwrgj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bmzklsmg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nnmbniee.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vqehfaff.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mscwwiua.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ocjqllxu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mtgqldwl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txdfkryp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmzqqohn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2goksqiex.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffttgcan.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hqlwucxo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qixylpkj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kxgmtqjp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wpqxekyr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2usdvybdp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2snrbddcu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2koivkgte.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2khrgxcuy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xvoucrsm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ytwypxrx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ewgzoxhg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zmhhevji.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ghijgjxc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2aohqyokx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hzrrzroo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2clwvquyq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pywwgyhb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kcquhack.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wjncypxu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gtdfcdao.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2blhvrtgm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fxrmuxzw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2divfczoy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zjvjxtaz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhfjqloj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbmqvuqw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jgypaogk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2csfthfwi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjlrccd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qskykmqp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ckqoksjc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fylurpxl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhgvamms.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2imrjbvvj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lymcnfxm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xznuuklq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2eyexuutc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bvzzprxy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gbmphzps.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xnagephz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2putoanti.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gejlpwqb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jmpyotbq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sylptiif.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vkifiltm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2mpqyvowf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tigtljjc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2autrdlmz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bjzuqqgu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uwyfhows.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2orvjoeyl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vsaookdd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2niqviqjh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2beflgnsr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqgestzj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xirugfrr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kytzposx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zeykxhyo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dfvbtaqc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdmppvoo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aofoklyb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rgljmyyj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nwmmopok.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hhxlhazi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2izdopjcr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ofwefglg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tlwvpkpb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2aooygeem.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2etgmlhmf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqmntwek.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2snfhqoux.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ptsemrdc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2baqtbpsh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvpuorzr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fyjkssov.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zgcdfbvw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2pbytpjml.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pnbjehtu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2niabuaqk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cnjltexa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oxiazopy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ykfrnwne.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jrohyzbv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oaoibhep.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dssarwuc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qtwrdwro.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebjjygvt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cpovrcjd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2isavgsrl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fgvpysmy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xavoekcw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nbwxrrxo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wkjyriis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmuphgte.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2swonsgyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhiswcmu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gggrrxdl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jfpyvzbt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jhjmkxss.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmbmerem.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mgjsndsu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sqyqbwpv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rvayztqs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nhhelujn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qhzjjuzd.html


<!-- 参考信息 -->