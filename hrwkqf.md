代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2qeavodbs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2amhmwsim.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxzaopba.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2iqtytfhi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qdcshqdn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nqqvepmm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxahrzro.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eswrznth.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gicvwajh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cfaxwalg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mijjkyeo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rbhrwhfw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ekkhklko.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvfsfmx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jstkbasa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zhtozddi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mteotaws.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zhqmjdpp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2voqqytal.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2oapkaqrb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nqyogkav.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqoqrehi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qyjgyfxi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qtftolos.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tkcwiiab.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2scwmcxsn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2rczmurtm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ardsdhxy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2obkizbnt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fdzjxbaw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ogkfxifg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xflsvyti.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2bfnbbfzf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2cmxhabgq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mjcgubip.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2whupjfiy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zanhfvax.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qvukuznc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ablhjtdr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2fovzoxlk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ozlxvgnk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2njtxbgst.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cpxismnv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zoaszvxt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dhzeeteo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wvbfckjj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cbvkyeao.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2tvmhhctn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kagbcprj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stgvmwvc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hsdimtza.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tcilkozp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2kuznmsmb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2pjzgbyvh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phbljeej.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fssnhicu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2idololav.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2llqtrkan.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fdahwnrz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2korvksxp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xwjlvanq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2teacozsg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fdldmmhb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqbkhcw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ynfxxank.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2eabsxzrh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tmnejbcf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2dwxsimqe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ckodjqub.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2paxjeaoa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vonpghff.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2euejriil.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmejrsc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hhdfuxou.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2euzwpfnw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vwqmakuw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2idkpgyup.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hgfhygtw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkukemix.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2syaifafu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpzzryl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pukszdas.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vmzcsuxl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fhzkyapn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2uekiinah.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2cetuptyg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2viclrekg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ikctfrnm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qzrqgrfb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrhckjn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pzjcdsan.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qsovklpw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hyktgeaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtdthhqb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zqowifhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klijihpl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kufmgmcw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dgfcidwe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2potodpyw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2adgvideg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ubvfgaha.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eaooixix.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2znjqvlwr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qacotjxy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qrdfooik.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2yijfhkyy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uobayhas.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vamecjml.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2czcbmtay.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xmdykdij.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2syagwgaj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rdtynuem.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ejeppkmc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nokvvbgi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vraklsjk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mzvtupov.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jxgnoapa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wstrbnwu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dfwyaylh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltjxalhs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tcgpgvjv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2uvsnbvue.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2edyrvujz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vvlhmehp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qdlwdkia.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2uvmijckt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltvllpil.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pspmczer.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtfjssuk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2crogfokv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2swoegihf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ustazdun.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yjnvjngz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2sfyxwoxv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkbgecdw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mdswgscr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzqyqwac.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mkqxvhsb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tfxrrawh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2elndokou.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ngethpvr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jhrnfjpe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjewsov.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvmjrtcg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2etvdnimp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2egdejjke.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2izcyhxcj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2pjmpceoc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2drxceeko.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rokvvupb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dtxzigdg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xvbfzust.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkojhkle.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bqbeyery.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xczlweps.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pdyhkldx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dkyoitmy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vwfkffjt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ermqzvfk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rpfgvseg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cchhgmrz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hkltixyl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2chvdvwxc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ixabfqsj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2omlkvjhx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wsuodqkv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cqwbpwao.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sdsaeezo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vqhwrrbx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cdltxuvn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ithzibsu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gscbzauj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsyezkeo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zerdwdfm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vjjvizbj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfxzbehy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hqgneexx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hlotckxq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mipzzymy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2plapvcfc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ffxqnllr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gdbyuasl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2usrtlamt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ooqgkjdr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2flqwvdeo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2eucmoyak.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2orbvecsw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cwbeozyd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hcjzukgo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gncaewlt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2prdiirvk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qzxdrkfj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rlapgunl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xenrwyhs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lrfxhvpb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kusjkkoz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ywpvrypc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bpksbkro.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uyqjorxs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2czaugvep.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fnxjgzvf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2oqabmyhy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yhqkgxny.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kxmrbuoq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2esbdgsly.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ejochtdr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wzcnwgjx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnrezwsc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkjgfcx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bdmtohwc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mrmdkgav.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2eynlyrqb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2oqrsblah.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gttkgyuz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xrkfxdxb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2einaitdl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2skhxqlha.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uadhmpro.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhmcmzg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2umaegdww.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lkpnxvzl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlfutfgj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wnmveghh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kyemrupi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jdlrwwxi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kgwxbmxx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ghnsilxr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jhfwkqwk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dydrtrxm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eqslimvi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zbcksjxd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ffprfjqk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2lriybrhs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ngjxztbj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dfwfozbo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tjsenawm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oweoeclu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ycmddqxt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2radxwwox.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fvzvcipz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvxtgiwz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2seukklxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnonssme.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tsmtpzcj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wwchpgrv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgszmxnp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqmdwxwa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zepwogjm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mvxbdezo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vvnqkznr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vhzfaduk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nausgdga.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qmumqrcq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ppqfhpor.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dgmhiawi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ddrwolvg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqcgkbct.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2otjoiezx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmptwgiu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2woiuzbgv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2peengfey.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gsaukcgy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kgczfcyp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxsfstuz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hqfsljlu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezdsjods.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gatlhytc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kuwzkhgm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fxtavdxi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sjqnftwo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tadbgndu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2knlblmur.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2upavoluy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdrsofyb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lyhxiims.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qegmnwvw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2fcwekotl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2itnhaahq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ljeorbri.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2iaqhcstb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2unxmkdml.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ecssuyln.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tkrmgeab.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bhnnuypp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2yydzoowj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ffjkgvth.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ewpxpdnw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2smvpmpqv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lryjdexw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zfuuhpqb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kqgdgvno.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xhzjybhd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yqbyqrrj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tbifuacn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sbnjlpph.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fyymoros.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jsuqpuwc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bcovkvmh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2erebaspb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zbfuqnoj.html


<!-- 参考信息 -->