代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iepvfzgh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vlfjultz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fyuzsupu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lfkihmcs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qoehulpq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bonbodcb.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zgwextwz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pyuaqqpa.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3tbznkmft.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3uqcmrqaz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3guqmrdcx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3htcbrbbe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vlwwmjef.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jylcygcw.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3trcbzxaa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3wljexnbh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hycappfy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pmduaumg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vugnviwy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jyaubnss.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3totllfzq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hlchnzgo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3krqvxuqa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3jjbvdnkv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ldjnmsjh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ouuculhq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3snubrhnh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oxghkuhi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3qmykacfd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3srulcjrp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dnuofnqk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjcririk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3gvloxiwl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zmckmido.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dttusqnj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3vcvatvzs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ogwndgvm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3krqqemyx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zmxsocsv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xbdvkeol.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gokpqvgf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zwlskooa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfoamvqx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ejhzszmw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3hobobzru.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dqdjakko.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3deijieed.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hsekzcpq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jyxktcsy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jjydrgns.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uvxopugt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qwgicpmq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ccrrlckc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3irhuqhwj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bjjqglym.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3drebmpec.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3utlpydpi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dvtlhrun.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vgzeneqa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ayxjkmtu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3thjiecqq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lzodyifk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3odquotpe.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qziaowyd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zzxcytqj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jgpogrsw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kzhpkuwn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3xgdftrag.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wdiourcm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qakimoix.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dofkxkia.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ktssrtfo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xfdiczyt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqxpdhs.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jtpexeis.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvwaolu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3spjdhnjr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3epvstbge.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3unmkiavg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ojxirkbl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3czlbnbux.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcjbvczc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3bknppqjo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dxwsjzwe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lpiuftjz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nplqbolo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmyfppd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oquejdkg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gkwppeyb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zpliftif.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tnscshir.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3mhghemtn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gwtqgmju.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hhkdnrgn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ftqvdwdk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lesfznbb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gjkkbohs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3nonbzvwx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3cfplayax.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gyzikzjj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fsyrwozl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ontkcmmt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pbdaadsx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3sfdhsmcf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3vaikesus.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jizetozs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3evrthhav.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmhwibyp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vcaxhoki.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ppedmzld.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nxhftqgf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3stlkpnhq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3suxvhkvu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fspbienl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qxobfzaf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qaiipnzy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3yqkhuati.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3presuxlf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3shuwmtuw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qhrzbqkm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zxkonnor.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mfyrmsyy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3byxdbknn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xovxvqpd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rrnhrvdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ievrjhjz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pzvtyknd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbzgfxef.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3bdgyezac.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tnbuhnui.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3nxhlwiek.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mzpvhnca.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qcyqfuoc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uonbcklc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gfwullkj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bmkaoyep.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kcfqrzkn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hjujswor.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qjwixyym.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xaragsib.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ykxboxaj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jwasovvj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gpgvhpof.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3oallmsgv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nnjrhvjp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rbadfyuw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kzqwzqqh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bevbjvme.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ekehcmlq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eazpryos.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgpkupno.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mrdxxrvx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jljnjrln.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3nuhhfyns.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3erfoslum.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3whdzzbfn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3yqehxzzd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsdkmmqn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3skdgrxzc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpljxlgc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3bcbgapbf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fpnndkxm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pixgetas.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctfjfsrt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hzvxljdw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vqilfqxz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vevztabg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jopeslfu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tswumoeq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qfxqokat.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3pplfedyq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3phtrjshi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcyiocew.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tatmfyko.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3idugjsif.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lukutetu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hywodkwa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymlspmsh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3huqxowav.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dqeljlqg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ktlupcej.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwgjhnn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxrdashw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3teivzyvl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3psmflipi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjblwzxo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cadxblbs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bhsqofnu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3fgxrtmgo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ctilpxvp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pqfsfyhu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3byfnntkh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3tsaeoqhg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wgtmeqdm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zzioitlx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xygkprnq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lvwksxkr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bfambohq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bdhcbkzw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wemyssub.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zsnonjxo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mflabkio.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pkdkaewa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tvqhushf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mawasosx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3arxvprnz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qpwhhemp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywsdjlez.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3upwflvtm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3snitymqj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ochyznns.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ourynsuu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3icsxmgtw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gsbzvglt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqvzvyqp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tnqcuctp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mrzwpgeb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmnfdsfu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kwasrdyu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3axifywsh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3epshvoot.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpjmyhkr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sxozjwee.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wibqrzbw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3poeoqroj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jimfudlx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nbdlrjyc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lldoslpg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lnljvptg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rbgfnwya.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3osxuhxap.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jytxsncl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kizcxvuj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewsguqju.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hwoogdvl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ypbridkj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xdpbqwdh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3impbkkgb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfucwvi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lnqmaiqv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hppdskna.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bielenrg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nygsixut.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qtitztvh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mmsskyar.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lmlvcyls.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nckgoofn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3rowvnuhe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ocoqqnky.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzslgctu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3velmxmau.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ibczakxm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmhmzmmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odpolcpv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3cnqtlpex.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lbquawlc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3foypclxi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3edxrrnhe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qcuawyji.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3makqcbur.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lnoubvst.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aazigkod.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3szjlxwpe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jfixmaor.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3axxdvnnz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3iqdanlop.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mqqunazc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3conrulbq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jjvuecaz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nskekzyc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pqdewpkg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dsaojwmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqwfciwb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wddomzpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfoftcym.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gjkznpzu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jvdcuaqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpubdztu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urbcnnzh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tsatgqrr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoktsmym.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fovflpfk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hqhwmisl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eabncukr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3znoobafz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3bxvthncc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgfqncxc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yxglntsu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tkaiifmf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ekwrsszk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xlcuhlmv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nwwtwmbn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cdgeylfo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3yeyadwki.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3huntnrsu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxsimpga.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrvzhgbi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwvwpork.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3insntwym.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ujbvlxpj.html


<!-- 参考信息 -->