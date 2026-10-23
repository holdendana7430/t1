代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ccohicyq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3trhqnkjo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hwkvamit.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iucqiwhr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xepupesy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zisgsmmc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ymmisgfd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3brtmdosy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nicbjrlx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3byngjkhu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3najlqlyu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ueuefotk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vosfcmrt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3siqymukj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3gxoqvrdn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hglmoexs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3dagfdmgk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zadjfmbg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3srapkici.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3uuyjuoep.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3imrcbsiv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nxxltvxn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vtkdbdyq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aqtqprzk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qxmjluer.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3pnunfhjm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3zooonqlr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmtqtem.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xwlotseb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ssbyrgvo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3jeutyaqt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3uoldzsha.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3lktqcuxk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3pjwzhoiu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3vifbcbzq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wipcvhuj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ovgocztm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uirnwyvl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzukocly.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kufefmzi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ttjmuexo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3weseckob.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bwgamzky.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3pdexfqlf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nxjtxvqz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxyumjd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ecyntscc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ydrfmvny.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rdnwrizg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3micoenha.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3hqntgbcz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3etqbhetb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kmawuqpg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zqgtgpzj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wgdxouiz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ryobzxri.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3inzueovs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fgkiorvl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gzzhlzla.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vypmstbx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qdxeybyy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ihwgetqd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3narmacuv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3agulsqzh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3adwddqvd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wbdhncql.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3arkqtplh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3phvvffbr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ctylccqv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cgncbkbb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rrecwjhp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hxixdyra.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yzghdlai.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3oqnjayty.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lzplbdwn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tftgkrjk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygoalbcy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3sqerwboz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qmefujkp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxwlmab.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3izvfhatl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nxfevbwh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3hzkqptbi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3govnjpfs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vkuaxjmk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tesqlucf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tzaftddj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vktujvga.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rxsisuhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsmvosho.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3isgcokhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpjuzndi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3nqyairpi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jzmaqtgu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akpzpkxc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdvhgj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zdzctyha.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iqcxwisj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3slyeftam.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3djhjxaec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oeuqyret.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kbxtsdal.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3bibgkoad.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynpvmibv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3riggerga.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iafhiddi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jdfxwojr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3iuewvsak.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qlwqbuws.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rqzpsxgw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kypweaiq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ajjnxdms.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wxhsjxbf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaadtftz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3utvorbzr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thyrpmna.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hirxzeot.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sdqfoalg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fjqnnsjs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aximfluq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bdqadavg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuwyighn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ismxhzce.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfuwttht.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjqxnzqg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bjantfer.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbtpwnw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlgbjwtm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ujfrmhws.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ezroybqu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsetqvdp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgbsdtiv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrccgiun.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsusrcqe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qhgozciw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mvgocoql.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3deurevdz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vrinovja.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3sbifxkda.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3iisyypno.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqeloxje.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxqlgngw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cffhryux.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vqqsfmet.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3savswcxn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ocycacuu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hbymgzbz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uefhqvqv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3osyqqsdo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcgnupw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jcgcxycy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bipxdgbs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kqvxpgjx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wlqmqkrx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwkmvgtf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dhoorqpe.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3lisbfajm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qtdgwvwu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vcqphheu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3udnqcbof.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nqewksxt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3voqnftti.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nwythvon.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3unrjwrck.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xxsxcvwd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3baippgzc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzxixuhc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wcdkoxeq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zkvqpuct.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgwexoul.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vwkdrgbg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftaypqnx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3adbsaqdg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ccqxgngz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gmeffhyk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3noljquwx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3posfxbzb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uvziitel.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3jgwxjxcd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3attdxxhq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wimadaxp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kgrkklrp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vtvufrzj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bimgsnjw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3srmmxjlc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ygcmprcy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jvvrscrw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uunxtrhe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nmzenyoh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dbssoomw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3scpxrdno.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mjzggnfb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3sfrbaksn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yspjcxqj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gstkmiis.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ojnzhuhr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxkkrkkp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpjkcprd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ezbrrdps.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3okgjfsjg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yinejiio.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ounoylvu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3exluckfu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fagqzkod.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aglejzdx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3baluoxuo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vgielidz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3argzlbgf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jxvrhstz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3myslymdy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mvwjfome.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gqnwdzxb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hwovhxwy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dosfrmzk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmsvdvvu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wslsvbrv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xxusykcn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lshjbxnj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3oxhkgqei.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jzlazjxj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lefocbna.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3krunodvs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uwkaoltc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3inlxnjnh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rzlitces.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3reyxgfuj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3egcrthsn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ojtaxrfa.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bidimgmr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtpmmwbq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ykqfvjkp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zuilyhnr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nzslryak.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jfbsmxrj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hbfowpdm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ocjhjinz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agzrjinv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ndgmqzxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvunbttf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3judbghsq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rxdnauhp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvdhnvkk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ubcqytah.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzcmowlu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebqsmijs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3sjlswxbz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3atowcaeg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zsunqcol.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vuhimnxm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rbvganjc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swekxifm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaymnvhn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cxutrdty.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3aqacyvcv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rlxxzjbg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3txxogqsl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3usimgihm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mpawnmob.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3esnojxym.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sojvsfbm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xgmqmfoh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3odygjqzj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxuaekph.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kianbgwo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3avrwdiws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jmuplbxa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qorgafoh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3prhghdpe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lodsjzqp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymtglbva.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3anigtadg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3kwoigfaz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lecgojbn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lcwthltn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3liubdkav.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ztphbrrj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ufeieewc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pfchdmux.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zwvnpgvn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zxgdhbij.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gspkixyg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pkvamerc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wytpwlmb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gjlmthzt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jvcbtpdh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3csmbwwfc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iixhbqmu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cbhjzjro.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gaueprbl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bortxddj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oxaigvcg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vvczzvnb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hjoavfsn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3icljjsqq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjvzccm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xjhobssa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lqrnfjfl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mvevbyvx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fyvdefmj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pqzjslru.html


<!-- 参考信息 -->