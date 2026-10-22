代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zadmezej.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jsqtdekm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2skhufhem.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wflmungu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2muvjvegw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2oqgeiwag.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qkemfesl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2irofatga.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2dzhjiudn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2jttiyaiz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kjjzjjyq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xdgwtdzt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jalomjjk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ldxdsbpz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2uqrhcmdh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yvrdkpsw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vpgiqish.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lkprpqkg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2igujaewm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nstxrfvf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2qbybdkyf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2kxgufyka.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qymvwdux.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jsuqmksm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kmxxfzih.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2okyexlzz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vszqzuby.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2mspqtxiw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2iqdvwdsd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ahemhedx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsfvomwv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmxyytcy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2akpupkzx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ipdcfham.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lqqiyovs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xhiqrnsr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tyvrqxxx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2oiaxterf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2idqcnthf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2drkyodqs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2exmoravf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fichecgv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kftgpfmx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mfuvltpm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eerbidny.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xntneojd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2nbdnemkp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdmgset.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2afxbirje.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yewlxajv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2weqmreve.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhgouzuj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hjkocdpt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dwohrfry.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2swiinqye.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bbhsxson.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lkqkotxq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dhapemmn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xdmikial.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ncflswrn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjlazco.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jrocysem.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hrtfzesr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sbjaiypv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zmvwplny.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gempzebl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uurdfurk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2olcryavs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jucrauvb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hucjkgvr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2zdrjzxgk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qryviwok.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2idigkoba.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2egicwsfa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2shzyalkp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2clvnwcvs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ikxukmvn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2utenehts.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2spbhfbdv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ammyelpl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tjovvwyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjbxliqp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zupfnmcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjayxcsz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xhdpuuvs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nsnxczcf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ifuhiibl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2moiwucfj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hhgedlpz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wrippszu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtsckaey.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ozdtkcvw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2irtsyyya.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ofyccmzs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2diwoawxl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esmpgxqj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lpsuytew.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xfajejig.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vifcducd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2uwtkywli.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uenbnzpg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mxzwgboo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nievsoyl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2viopyjsg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cbpgdmtd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wjmqrcpt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pfpghvth.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2acqhjuqr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yeebcakf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2euvmphil.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nnirjoxi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kjljgqri.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uaawrulv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2voccpsie.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cewgohxc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rpyhrhkc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qjdaggpw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rraxeqwu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rpclfcqb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jaywmaes.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mqxsbdgx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2elhzkgge.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfkgphpk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bycrcjxh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aoirvcel.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vumgsvjr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qbvlxbov.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zymrxvfj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2twrgjkbu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2sngtnkau.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tvjvdang.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gyqgpybi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2awhsazla.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2owmbpzth.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rvgceicx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qhlalwsv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2abksklmb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvwgsvac.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mbmqbxzp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zqjszxdg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wtllnffd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cgfatgak.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztanhaia.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ctpigzku.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2witoooec.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cgvammoy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sxyrkbar.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rmarjdib.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2huwopscw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dxejrysm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgroobab.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ghwgcwpd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qyvgzhdj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kfthxtcx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2csczvtjg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ncbuhbak.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2psezcbon.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vcskmuzu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rogiujsi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2avejqqno.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mugptzkk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wxfhzfif.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mtrerrhj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2oqrtjyyw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2epqunhmz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jivcazzm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pnabbjxl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvxveck.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yflnrbka.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dcjheomm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zgafqgtb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfsyvxs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2karubdpt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdrmnbqv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rfavaykr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jjqedest.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbhqdbnt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tzpbishq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xwakfycr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pbuqsuqq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yvcyhwtb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ydnvysmm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mplqlmxr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mcttkgfk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2onprwfga.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zfemiabj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lpeemyor.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uqerucgv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rgjqxmbb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jooqxasm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2scupmdxx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aczvnpio.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dutozplz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2caofuuaq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vwphhrfk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aniekfqj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcqgcsu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ynknrfrg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kwumaali.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yatrlwjo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hjbxxdeb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xwotdjpv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zulvsfqa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rruxwtyz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2garunigd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uopidxvj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwutcznx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvvrptks.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryvzpvaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ejffjqqw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aerjehso.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2glvcaefb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2isavkwas.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2imwclfiy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2quecqfpw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gkmqbgmi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zduiyfog.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2allzmfoz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wlugyaga.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pauleylc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qqmyuxlr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujakakyr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oxjvxqxr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tcuruqcf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2origonea.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dvpdpngo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2gdnfptpb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mqdhvnek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhjwdwva.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lkmeovtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjyecbjy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrzxxhnh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jiqbyjpm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaopzalo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjgjlkpf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cyoywizj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykhttshe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2deucfxag.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2laanelbt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyyvitsa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2axymctmr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rmagnuvg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2punjpppa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtffajlo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yjqjyntd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lxqbfkrv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2avkgpywg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bqxkkqop.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cqrexrch.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zixqfqxc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gjgncjmt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gbpfeuft.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2luqtfhkj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdlmhfow.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hsrbhfxc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rylzkgnr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2amqqklfd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2opbqhqzq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zxeddkmz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhygwbrh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ljymzpws.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yctrkftr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mfarjpst.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qotdoesd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yxagziug.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rjrjrfyt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tkjpzwpn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nvrwuzyy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xrrccfvv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2piztkpxo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nnyvmmld.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ahlwpxin.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ryqeoend.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ufgojuqt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xzjbqatg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2awfodkya.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gddneogp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2wxqpaajs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2skswpnnt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gyhwdqcv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2naayworz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zamqeahk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rhsctbcc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2oupfxzqh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mluzvngp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2feyaoeus.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2xhqhdgtf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2exzhuufw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hckepyrm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rholwvuh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ifrxlcgj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yqwtblrv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vrvmolyy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xcqahwli.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nujluusn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sxekcwkz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2afnxlplm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hdmhwpce.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mredmvrb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2asmqygku.html


<!-- 参考信息 -->