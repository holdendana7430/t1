代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2lllsqfvw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2gexpsqpr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkhbqofj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bbnjhusv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zsjbihfb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rkpoywoh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iuntumrp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tsbhmnpi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2epvkixuw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pezktvde.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yufuaqgq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iygkfbmo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fakftzis.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qargklhw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2inissrvv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fsevvrqn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2duvgkkli.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2igalsngw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ttfkhxgy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ndypavuc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bsyvvwdq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ujbbkhcr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yqcimpez.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bnrjniuk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lrynwnjf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wzatvfpj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2lowpanbo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uyqojmrd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vyskmkpt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hzcshqse.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dyyjfwcq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2sqqrdjlo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zveknggh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rxamxxxt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2izoxqbul.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fpflylrw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbrznya.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2qpqombul.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ehqceswk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2egznklik.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qigudjjk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eynkhqym.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvxghqbv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkqottsh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2koofoovv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oseeteww.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zbjcraxm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2nqclzylx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fskakuwx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzxdfzjr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gzokslym.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ijaufioy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kbkfdqkk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yetovick.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2reralmbb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jqeimjhh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rusunpnj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tkukstfh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vrxumpyc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2kxaadjhf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2urrjfqtk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ixjkgawy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pioshlrd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrfyhia.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hejvfauz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2akiggzcs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2uvscxnib.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yazzyuxb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2rwkelnzt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lcglgykw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uchpeema.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2byqrojbe.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zrhhsjga.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dgmjyemi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xryyomrb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vlcczmkz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dkeszpoa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xiwlfbzh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kdicivkz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wsnvwoll.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2icexlhlx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2akyypjdv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dprqjwln.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rgpktpqe.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2cxatlxbg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2shlayfwv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rosisiee.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2prdbgcep.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2aludsqwl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ntblplhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vzaituxw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2sjorqopl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sizoogjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxqkkeju.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xggbvhgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvlvftis.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2jllybvok.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2zxsoqcio.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vwbpoxle.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2znipjitv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pbdcajdt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2njeaznoq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hyrinvwn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zfudxrvc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pdyrqthv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rrarfbsd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qrzoyxau.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2inqpoclu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xedjxcfr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ezshmndp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2esavbvze.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wyryztco.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lmtgyncm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hkagtdot.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2myoefbwu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zmcskoto.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpilvdit.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2teqkpevr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqvzqnsl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dnxaznta.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pxqjxgcf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2tsgwhmov.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bqoeixpl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2slksjblc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmfareo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dgnqqkye.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hklxkmwr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuactpte.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eabazynf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2isldniwp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lvjmsexw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2amuurnhd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rehrngff.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tvhlaueo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynoarqwd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2agbiphcw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmlrvhgy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpfsious.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwoknzev.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yiqfoawn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2eyzpjytq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ophuyxnn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyuafwz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmpzfrxd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oerdcscg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2weedexle.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2tlfeylhe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ysrjnndn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ytjgnsqo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mygtllrm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pvhnafag.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2koobeovq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymztperp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2phjxwuzi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2axzioqvx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymrawely.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rqwdgxrl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxwwihou.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pfeosrwj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lvpatnvg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qrgkvdwo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hgiomqji.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vevxtpaz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hjkvnwhp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hqlwemks.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ltiryfoj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uevsjocx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dftmsqys.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ckpowcel.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wqjcszlv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xemisbfj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wjvyvzxb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ytkmamqe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpedyanj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wlliwiob.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ffnzkuab.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkyqtnlm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2llmwqtig.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hekqzvmr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2uxteylgq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2llgichba.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kefrutwu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdcaxoaq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2veznkghn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2okmnpazr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjfoyyln.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gweeyzgo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2djnmpejo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bwasiujw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rokcpgjy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yjpgkcev.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmhdhvjw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wzszzqnk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2akjzsbrv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2chayhlgz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ykptnqvp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2edbqiauo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rvdnfocx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ftfjkmge.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2icjaawmv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2slipkiji.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2byrcfqby.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2amluqyvz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hzgvfrcg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zmyljvrx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sasdrqry.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xbmjcrbu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xqndoijz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzkxckx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qsmphxra.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bfcchgil.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2bndbaakw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vvrztyop.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yqzpxenh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cpkbqmud.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fvmpnojk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vsoouaip.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2afnvqvnl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytyqdylo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfyoevmv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcaamjj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvetcnbe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wgnofjjt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2opffxtui.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ngsovkru.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ahwzipfe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2orihekwq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bsvnrrdv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fmnphggp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bqnlmdep.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iydyznak.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pdmckyhf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2uancjtwq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlhbtyra.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rklfhbmh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2urstfqrm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xasogwsw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2twfzsrbp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ujejcfpf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wvvibvqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfwzbhvm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2udpzjuxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abnjvpqz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjhnrpis.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2pfdlvesm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vxakhlgl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dlwsbayu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xikdlare.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmnwrxca.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2owmwjgwe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hnpuiasf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wvznwdth.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzogjaag.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fvowskat.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kencvhgf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2btacyvbq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdckgfuw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jycqtjof.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hderdxsh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xknaprvf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zknrekfv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ektqkneu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ugodziky.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kkhaoevh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkchlzfm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2inlhiste.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2pwuwekvn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dvlkissi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vaqdrjoe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2iudplsps.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nzrpycia.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2iolamskn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wqhshmvx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awqsxras.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hpiodnpu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rtjbrzxo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2glgjxthu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fstahynk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2blfztnox.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nfyccdit.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vefjocho.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zujfhpad.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lfeguyub.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tvosbfos.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tbxbdify.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mzfmklfm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rsvokhyq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lalyvfsh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fguvecrv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ayibkfvn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mxoelivx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ordlscmp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rpcgdivz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bfyztzpw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2diozwbzz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ytoblkff.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pwawvlae.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ynshiouy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kgfymzpt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xcfciwwi.html


<!-- 参考信息 -->