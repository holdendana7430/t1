代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pylktswr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kbdlccvj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ogykablp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjuedpr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jvhcnoqt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nchcifus.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3bimruvik.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3gwhtlawz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qklwdbhv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jxdmcmzn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oaxagkgd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3aqnayqty.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rjvlklks.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gukuefrr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3elwqrrmy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qckaqelo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dhnpyylc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3eyuzjyew.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3fkuhsyji.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mqvdycdb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3eieuafwp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3exbwamaz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hjnzyfzm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fpjsewme.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3pngezynj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3srgukxvy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xaczrqol.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vtfhtqgs.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3shvjkzki.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdymlev.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxufilg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jpqhwyak.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iyyuosud.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3depkrqve.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yuuikluh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3bdzfpdym.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3blszkwct.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyckwujj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kmgperzr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3kgxrcshy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3okoyyjaq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3hnumphkv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gwucpgxm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mhwdsljy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3exshrvlk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sesabigl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qmimxjgk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ikoasutg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yeqyofuz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rxfzorun.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3obaensqc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjonouqv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3aletkomw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ujqyjsnz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yzntcugv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xjlmvjmi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yxgofrbv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kytxjpic.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pchnltgz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3zjlnczpl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3sgckzvkx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3hebbwkyk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3avxrajeg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3smezfemp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wcjknqyi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tbzahhos.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojcwdrzn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3otgejhte.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wytncjxq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hfsktahd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wfxzczxq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3myfauhbx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ttxwnkgh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yaacmzrl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mpphegyk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xqtwwmjx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ardwrnmc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3npnciigb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fivjoptd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ftouhoor.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ijahlzak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyjdvtxe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bjttltvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aglrhnyi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jajvmbuq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lvvlnxic.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hqkxwzsx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vjahkato.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eeqolquc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kveyvsme.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mcayyadq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3egozirnq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dkehfgww.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3uuhzirpi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3nrdkhrab.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3glyfirpo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kzqimamb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gdbglqau.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jgihkczb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lnawuhez.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3olsnqbtz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rsbnmxnw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3myvzbfgr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ofylnpre.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ffcfmqjz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ljwapncm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pxygmcvq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckrljpot.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhuimqw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hkbtjqoy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mkxhzdte.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rhypzpir.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzebqgg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lpagcoea.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zhzwefbv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubtszkaq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvdpdgme.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qgdzyfqw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3iycjfwxx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fzbgucvd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lbvdnhdq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3umrnizui.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3etophtas.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lhsjitdx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsjaqhe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gsxjogwj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zxevkwel.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lycffskm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3eabrrgbj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hkkxucgn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwvoeng.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jkykfuas.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aapwjfgk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ijxkxvtg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3oatqjoiq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3oazqkgcf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fhqvkxik.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcbhjret.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vfltffnp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dvliyvfi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvcusckm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mxlqirct.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hximjxpl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzshbecp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3biiemysy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pzwmyoep.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3prjbynum.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3elvzlknh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pnxaltkw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hshozuwy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mjipkffe.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3scvkhvuw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nvjnrldu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3enolfvgs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3emnkgkpd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fatwvien.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3orzraydq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3flnnjncw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3krunrlzi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3unylhjlr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eavovmyf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqwxrtgr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tczatmvd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgxxtadc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyskqnuc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qkhqkmwg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqbmvsu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttnjiodg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3itnkygzk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dtvkwbca.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ismuadkd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tqgejrqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yxcbmmni.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqhmmbxc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nwmcjayi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hhntbzbw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ehiurovv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3loolejgo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3brozgood.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lurkpcbz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wwgcptor.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ynntakuk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3anttxcuk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3afozugox.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hrgmjqqx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mmnlgffy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vxmyklrh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gdtdvkqj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3krwiibvb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wfxrxsth.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3advvuwnb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hffwouxd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jutvaayx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gtlahsba.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hhmkrnjl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eypoucxd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udcdxkyl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dxbksycg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xrdvrkdi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hgmniyfy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bbmtkjyd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3onbuodfj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3erjhagvz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zydqcesz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmonlah.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dznnmmzi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwrkzuw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3izktoefk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3unakuiun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzrhihg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nzauzrwc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uybvaltt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kbtfkbgc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3erlkroer.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3krelmsuh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jqxgqhoq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lfiieivs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qrxklqrm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zkptklzw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rsotpaqc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3btadeotr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfyruxce.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nxxdeqrb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3htjiesuv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gkssgdpa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3deujdaxb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ebemhfqb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3luaqblzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwgsmuub.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fzlbwvip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhhpkloj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sktdukln.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3njbzxunl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zlablsez.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqpxjafp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vmtlvxky.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvkultje.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jzlzgquu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3algnbcvh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sljgoycu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vowvemmb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tdmksjvl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ltmvjbcw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3euoohwav.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zmatdjkp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xbvkgphg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3uztbmzhu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dememkpg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nndfubnn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rdjgtphb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jdcmmonp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynkqsaws.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3augjmoyu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kexyrxns.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggwhunfk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fwilopyq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ygzprlwr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lipudjnt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixoblkzz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mkzfoego.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mowxfnhg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ejfdbcgg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vgwfcbsq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ymbtphhe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nirgoipr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zosnkagf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gbllleqr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xnabwnaz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ktjzhnfi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lbkappzs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yrtvulxp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wiiatjyy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jkmgtnuh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ruwajxjl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xpcbvtaw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xinczxwk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qeeitvwr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jdukajzy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bbgeekgn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fajtmmsq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ezmaiftp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nyevredt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tqaknnqr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kfomyrbh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wjmxgexs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mjinggut.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qwknymvn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dlyewoqt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3uflcueqa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hacmgsqh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fyqgwkkd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dzswlunj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ukwadflg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3heterhvk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kclvligu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3uoatiuqu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohkbwrlz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3beiwmrfk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubewqvol.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3meibwsnd.html


<!-- 参考信息 -->