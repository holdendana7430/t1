代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uuzpfozw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jwnliwpu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2khmezktl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bjeylolo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ejurpyua.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvflokzv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgghlryx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2egcozbbn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dlritskh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2okujxagt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xxxublfp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ngbomlia.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2akrlwkav.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2prnvdqwi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hlhqyzvw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rxxewmnd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2kvjhimty.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2uldirepy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kxrljeym.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2uejktsnh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2epximobz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jcbjfzpi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rpjwezjm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vmkijinb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kurajady.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2enkluqwt.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2owxygcyi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2qlqpmpvj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qqcdeckp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2iimqvllp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2aznhthex.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ivdeeieb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2pucuwepi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ulwiieqb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dxsevhhp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vbjxjxlr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wmtukqpv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jlrbakti.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2smigfylv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2liwkqqic.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2urjuqhut.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2urojnfpk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pftcxhof.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2yctssxfj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lcgowqvw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2czinfvte.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hixvaslo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2cvkaiymp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pllofvty.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jrhoqind.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eofqrbrf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ppwemezq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qandmpph.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lynpyrni.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pwnivhrh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdjepiek.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lxwyxett.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ksbrzcle.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pfpcpcsh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2tcwbqemf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nfgkezyy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cqbmhbnj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hilhnxcl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gjtvnjbg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vsuhgrlt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tapzuqzb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lqqydfim.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jftqgmfn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rzihesta.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tbpplvil.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2eifmlzdx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2syagtuje.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hfczezlb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2siypmsww.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rxpdqimx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ufvwwxeg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2whhosevm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lvcrjmgj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ttewphal.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2escrxtfx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2eamssvtt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2eblywmpn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2mqvhiaje.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bdgpcvjj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2vczhgute.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fmteevmu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2exdlebyd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cwowvvtw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qwiygdmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibegnrjv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ahqduvcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shpqlanz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2luosecau.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2sszxexsp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hmxudjsj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2radaelht.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hffiepjs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zzubomwo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hrbtfuza.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xqljuxfv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sfbyslsg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qparofyy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2rqihkuux.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhhgksjm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fdelajkd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ogssxrlv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qxrnwecq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lmbpjevh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vptxmspr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zznaojrg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ymyvyxhc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jxemoezv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2avfhedox.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmkhpwj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vvuhcwwz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tqclurti.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ockbzhkm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zgkffctu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xtpmegog.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijzoomkh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uewmhbxp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kyatqbja.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2aqgnokxs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vcfwqkir.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2izqkbzre.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncebfkul.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pezfhcqf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwqnddrs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hduwydku.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2spigokfc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmxxhfw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mdeohghs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvpdygnf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ktpikbac.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wwezujlw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wwuhpwwa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mkmgkodp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ivtxkbts.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2foeusfvd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cmioujjr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwaibubj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xruioijc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufaxhert.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgykibo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ujwyposq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhzppwak.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hnhwfksd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mwnsezzq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeqvpbiu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wutoedyp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2diqwjbkr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ulpfmalp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dkhbfcfm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xuuamlro.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uevjyhzb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mzgzlzqd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mudndnar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2elfzdnev.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dmayyzec.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qusqgbfd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2chrvhtzz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2otifklvk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nqpxtrfz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qewokkoe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uyifyjoc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ytxhfevi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yexkwuzd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ipibcqzg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rsvnkwiv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nxdtvxkq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jcnhybxr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qhxsbzak.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzxkmsw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2khwfcjkn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tsemsfan.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qulvtbpd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zznujxbw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lhqhhzzl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qdcrewmc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kaphrbfw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mnamjoav.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2kihjyflx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hivzshwn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bapgeugr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tnofnwsh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vyuhjuxp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ansabuvk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zwdkzkpf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2avbvuoqf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mknetyoe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twmbusgn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vddnrnoe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vtkthbrk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ykgvtpfw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkglkih.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lppiisey.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oidzsquf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lnalzere.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uztgfcns.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wveflwgm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2evzsrvzr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sccwhyni.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xndlutdj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2looquuet.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kwwytket.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2fhdffirf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qohtgftw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nfcxrokt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hgvemuoz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fiepnxph.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ietnwxit.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gilrefee.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kundusip.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2phvjpccr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oilauquh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwrrspce.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swlwqkjp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zcxuqsio.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jemflqpc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fwzlolby.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2anefanhz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ofcyxryf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gjsfdxmm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2blaqljzf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xlvjhayg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lhsgzuhl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ufgrktle.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2eqptoves.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mcjoafrn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2drfndaes.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2whihcmnl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bbxvtvhd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yztunmiv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nohwpsrq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dscuvuje.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lvprlfhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktsoplpk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ehbeshuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvfddyvd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fxniwbto.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mkhxawhb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdfwqqmo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjphfflq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nttyojhb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2agedjsbj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2coyubxvy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2aorispdi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahkmxgrc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vyctkhpn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eftpmqqt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwmfjdmw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvintxzb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysksdeyl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2fowyzvet.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pbrqgyjl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tcdorsud.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tjezsfbw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tgpnfbqv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2shkqpzub.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2arzptofa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpvhfkln.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2edbyapmv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcpfhzvp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2engcuzng.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2afreyarb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nzojjhnp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bnsphotl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddmuardj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftnshsox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gvgovpcy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kekhwbkw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tpddqbjl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nmegnafz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atmonxmn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgyqeha.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2msvtngnp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zuurxnjt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lodxeqcm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2anutjeen.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2phisudml.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xeagtrdw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2supdqkas.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cwuyyxlc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hvnenfjm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bbpvqluh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2exuojuzw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nxougubz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2axfopees.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iooqefor.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fwkumhsa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fodegvxg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vommxzwt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2boapqjqd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vwthzghu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2soxwnbbf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dudojsjt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rcduakwc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2laftqrdv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zcokyojp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ozkzrwaa.html


<!-- 参考信息 -->