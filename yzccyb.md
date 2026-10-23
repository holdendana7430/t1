代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pppjmksa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3taobzhsd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3litdmouo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bxrvokpv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ffrzbkas.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3duknxcni.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3toczmbrn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tgnwpibx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3edckyega.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3csgfgjxl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uymwzzlk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3seopskmd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3foonmtwx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3yharmukz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kabhvexr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ioelzegr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3trtklpak.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fgkydjrr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vatunhpg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rpieybyq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hoeyccal.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3fydemgwh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3cpndfcyd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rcfaddat.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bebtmaer.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qbshkyct.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bhaxqmcl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3uvfswqkm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkbdeku.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3aqkdumql.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3atgftblo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3iccghrrz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kymmxhmp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvyvjku.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3auzzcqye.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fhgticvh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zbbcwgfi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fgeexyye.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fuqjwgtx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xhoavlkp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3klwgryvf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3phmyorjd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dydxyimm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3gqpplkco.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3kqixezqh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fjcnmbjq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3foahoxyd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cwookhxp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3evvqokda.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ymzzvqlc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ypbwykfc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqorarnq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gwcohigi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uvxdgtql.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rrprifqw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wcrebnhf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zolneqgd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3atqorphr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mrdfyoyy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ebwivzwv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hpgyoqxu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kvvchoha.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lvtmdhry.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3tgmhusme.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3uolozcoo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zqtolkpe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ccyeljqb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ltmcqajs.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tyerpvgz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ufmnaald.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3prbvbkud.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3crwtrxde.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3jpxzaexj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxdvonc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lozeiawm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qfallysn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hiqwhyua.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3hffnxgdq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3gvmpexyx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3dmtqpiog.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fvwmeadg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3abgqsmps.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3cdyoktlk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3erhkdkdh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gofdawtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xutguezm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hwkbeglc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyvlmgrn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3szdkgwia.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3awlumcww.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bglvlrlk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xovvjfxx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3onkktxfh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3raxbkons.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lehnfotz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xkbbrkbd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bwtagcgn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yrroxxoc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qtugibnf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hremnlsl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3siiftszi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zfcfavei.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3drakgemy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3oroqqeco.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jueeplfn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3owoagixl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wuoxivxz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jiewxney.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgkzzgm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zppodbil.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bgqzrxvc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkdtopzk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lebxdvzs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3urvzzrmp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mzzllmhn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fepoaftn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mocauvnx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yfynkzmo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mmagumay.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fumwbtob.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lqjgsrkf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsybtrm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qsknllcd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3diwururs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hpmckdyk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ldvqhnwy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxiftwkv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbokpgjt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tuwzdjlp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ucrfagkq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mibaqeor.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ltxzidft.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyyhsiui.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wazzdoop.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lfwqfccd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ubvpvnid.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bcsmhdtl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tbtpdkph.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywogdcgw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ywvapuof.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3iimwween.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dfdpgkfs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tlssforu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kvgichyz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lsxfebqi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qquvjsjk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xrbstrei.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxohjwfy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wkclvrew.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tanevvhv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qrdmrgme.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uirojboh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ebtzftvj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pweeqsyk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jswbvgbf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fjldcmmg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3orgfzmsv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3alnwaaue.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fymgyvft.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pgqjnrns.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3eccxcxlk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3veosksqe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3blgrgurs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnzjbxuj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3syxqkyqn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iyoyamrq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vgxzlpkw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtdehhe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jibxzmrb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zqsnbgpg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3kxxokllk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qewivprn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3niqgatia.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xpuvzsra.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3sazhkwrj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmiiocdf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zsyiaooj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zycgkufx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cbairnyp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cftavwiy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clzltfil.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hwusulro.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dgxygniv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plzaolnl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jstlemng.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mhsoitrv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cutnerqd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jsnlyvvk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bflscqot.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yzybtkip.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pgetrbet.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mvlbmrsx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gskojwgw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yapthlgs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cqtedwed.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rujrblaj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jnmjowak.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hwkertyi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3uibmsebd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqvthfiq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhvjpbz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hhujdsdf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wgepantp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qaycfcry.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3egqfddlg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qldirjji.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pbrflbmq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3agujaewe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgqxzuj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jduwqpgh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3caagmrvt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhclybpd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yyoedfzp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ifnkozlt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vitpmshw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ausphrej.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xqbdsxhr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cxnsjbvd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jzxrdaqr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jkzpgdzw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nvqtheoi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hqmipynm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3msnzkjqt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mvxodsse.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ftbdejry.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufhoxvws.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iioqjdjz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pklmefin.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vqtpldau.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3galwqnam.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ntgqyndo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3skwrxmkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdfnndeq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vqxmkood.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnswoi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bcfvogez.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yzibpygk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kkiwcmvm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ixfmdeed.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqyugiwg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohhofuxv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ruipfbog.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3elownyfn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3esondpfl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ugjdgfpm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3odgbksdv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gggdaklw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvupeheo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eonakizf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3itqtxyis.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjipmrrg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mfeimyoo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mlbvqfae.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lucrpall.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlnqaty.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cmqrcmvv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hrsichdb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ixuxvobv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wtamsayz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zxfoudsq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3slzfkqcz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yfsouleo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3aflhhydo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3fmdxdbyc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3euycvcli.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmcvkzmn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3awphsohs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xibgzowv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wvbunqvh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmcsiztl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrhfezk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vuqtqelt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mulrpzcn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gfcgslse.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kamjkaqf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3varqbrps.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vspqamvc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gpynotan.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bwhlpwxa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gpqjbnfu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bpkglydo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3luesutwf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bcfzchoz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fhvhmprs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pmtmsssm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zugebvep.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3otysqnti.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wxbdrctd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fwwtuoco.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wzxapikn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3shewwozv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ynxxsuca.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lhotcmoj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3gtxjhxsn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jvsuxuux.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fzbvuwny.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gleppjjg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fgzucgzs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ahddgkny.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ruulacmu.html


<!-- 参考信息 -->