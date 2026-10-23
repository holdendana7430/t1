代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rpscmqvw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xhwyohra.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fjurzseo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3gjyfpwgq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rnmmmjfv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rsdqzhqz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nyrjjuur.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcxgmucv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nyrzcpfl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3djwanyle.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nsttpntd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kgocczzs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xzqfhxlw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbzobpp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hurnomtb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3udyfosco.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ltvttjta.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3hrilxils.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ivorjqdo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kovelinj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3niyqapcx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zfyafzbx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fhvoyzgn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vxiuxzor.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vtburvva.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qzhlhjen.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qrhxfdqg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lovvkqjm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ptqoujkw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zqucqnza.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3nnxqscoj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3eozosonh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jlsvzrwa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3cwkcesnp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3usqvnavr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3adpybckf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ypfhrcmt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tsszyaqx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3gubuirmp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3cnfghnnh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tuevhrmw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ybcdkwvf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3myvevidb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ntdlfhyb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3woxhwkrz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3czoxfwnk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgfprgd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rrwlzfxs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zuyhelyg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqexyoo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ceytebiz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3fbifqsbd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3axsidxry.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gydtvqrt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3pfeuvmaw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3bjqiwxcp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3lvnrxmkk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jbjsiyjn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iteukbmy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtdcsgxb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jcmegrdc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pzhefiiz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dhipreil.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3cbgxmuqf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wipeileu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xqkmspex.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fdbrffxz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pqjrpnrs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vgznqomc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qmtxfegr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3llwxkkbc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3bxmmqnnf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3poarlwwh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3akdmjeqv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vtaecwmy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iuprlwxw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vkskcjme.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3byyhatrm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvtopbc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyensya.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejlhbibw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jpsrfqal.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ntrfiwtx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nvytrhys.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gznqyuid.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ylekhtxf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pcafwqkr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3irmvffbm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3quyqemuv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yvpbibmt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ivnrjfgu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bcujiccv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vugkdzyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adwdimjb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pheqmtyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iocamfcc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xsacjolo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ebawlzho.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kybslsda.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sfdkypzf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nrnklmml.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iqqdslqn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ecogifje.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3hiwbnxdb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dorldhcq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qzmdhgbq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3teabxcxz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3raqrrsjw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pyegorlu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ozuojvyu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tbxfnpbk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zaivxvrx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ywmhxanx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zlgesvso.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qdrcdbqc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3plmsphbv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrrfkdqu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctstrhqm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgjjkqsl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dgbwgrbd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3danjwtgp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3kajmddss.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cvfolsqf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zdzvsshk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3stdnavmx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vhaibybt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jumhjkwp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yltoovct.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3sendtfjs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mkcyijck.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jklmcfic.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrimmzxy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3irbehjts.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3cikhlkwc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3iyltbscj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghwwqnvv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycivfueg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3aregmnxr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gbnawalg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3czvfbutx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnremqbv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xowgvvxd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3grxvswxo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3oavxyshm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yvwcbtwz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kwsxbekd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ralsyxwb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxdothxx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rjoijzlz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdrnywso.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gciozozz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxmxjuuj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgtmarpf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdtgkmi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gozxahth.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzoundug.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qzrrkmma.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufinrpnr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxsdkaad.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sewxvlqy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jevamsts.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vuuqwhev.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xapsbmfl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cmltwrxs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pjhbhgwh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fcsiueow.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hljwefpd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qkkjslls.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bqhtxmkp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fxvlprgb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqutakgs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3efgbrror.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rblyqjyq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oindhwxr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3csvbpawn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqswcprp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3egwpmciz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3thzmciph.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ngfahqvw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qhqnljvl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ywhumumv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tkxyileh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3awawxxib.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oehdezev.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ezdiwthb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zgmwmful.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mxdngmoc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3vqluqhzo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3esswezut.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uaqmjppk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wjtnxhro.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3akcnfbca.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jxytpxji.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lszbplxw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3flnuqghv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jlgglavh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3moakmxbc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sfzqsyim.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvnvnxit.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qsqbqhvd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kxeunhyp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yzvcbyni.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3bwvhekux.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3upaozelu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3igpinsev.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ohofttxj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3akpknikq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3otrdfzcx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awamurub.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fdspavwg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xwcnkpzq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3cobrygvu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rahktcun.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3miyaqbdv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nxekpzbo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3glnzundb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkcjsjk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhxbfjhh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3arshjvpy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zovxvhiw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dboiphgs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bbxayluj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3olrbpvsm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gmdaeerh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3etgbbduu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nkfyekmi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uvgkxwdf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ehjqjvoz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3giibrmsa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pidikbiv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ujtvzxnc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uutugeqo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wuypcwkt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqptavmn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ncddetfl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uulaltkn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cwpmcrjy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3egxvdlsx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vrckzwnu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kqerbglz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slinjiuz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rpzedfhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnhdnoxg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnuqttvs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xisszeyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bmdwrram.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lwjksdri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktdyjisv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofwfuutd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fuqdprkv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3spnsjide.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvasjkiv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rydoxdye.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kzartsll.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlazghuk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxmdsje.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rviexzwk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bcgclzxu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3drpripdw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bfwukwii.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zwirnxqv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3upeacwri.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qjmwfphp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ymvsftiv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuihdmfw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zukxkwnx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddbpqjjr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3suefritw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ontueqtq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qdoboqax.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3khjwdcvg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jnghdikg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3izkaavkd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmaibswe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mzrafvzy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3snubifuo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dfiofnvz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbexqyuf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fxpqcxqr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vcybwmzc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3piddqscq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cmnfzyzv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ginpmxjs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cbueaypo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nyswuvvq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3swqcbumq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3igfnufzj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3louhrryd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wpmqglmc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3guhxgbgy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kdygnjll.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3laxmayno.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ydpgzaxb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ckiiwdyz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3egvmnmfo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xtypzgfi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tsajsqsv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3erhxhadq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwwngwl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtvbwesf.html


<!-- 参考信息 -->