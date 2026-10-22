代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2clrqpepm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ctwqphbt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvkvty.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dpcgmtff.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2xkhreyps.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vajdkdir.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tapzplxv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rjdzrbkb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2umuwpqhr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ckohoqzq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2apsxoqxg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cnmxrjxt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2pcecbyjl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2njpnfvjp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vwplblkp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kcqenqzm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vpgzevcb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2flcgthyx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2gzzobpha.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sjcuiiwp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kefazvgg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2wgsbjiqg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zfnkahgk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2arsntckt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lvbhnzfw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wvirrkiz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gsnqjwls.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xhomgrit.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bbbdvyoh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zjtnejoi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2opgxfpua.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uewtzase.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlcelrgi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bkylotbj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2teunfsmq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zthbzfmy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sqqhotuv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmiyfpx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yetefzep.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lcbyyprg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2smroiaua.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2mzxgbppq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2fqqcqddt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2gtxoirtp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2kqgjpgsz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qbsmikzc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2kikjqjqh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2horuigun.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zncgcvui.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gorfumvx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2mqztojav.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dxzkjijg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ilmehhsc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pqchhxix.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mkjvnhfj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fjyggkhp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lgejjueq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bgokmfap.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kugjpdig.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fyzjyivo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qjkfygxq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bhqdwjsa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xmgdepwb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cyungutd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdkklvr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cugqhtev.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ettegtzm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vzgwcapb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2sxvvnizq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2izbqfcei.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rltisnrm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fxkmzwme.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2claporko.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2huamrcmr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hnqfjwhf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ejtvfbar.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cfkqhvig.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xshnnpud.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nwjbahqo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ilyyceey.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2abqxasgp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kvztbnjr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hecfbsik.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xavshteg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2suodgrmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwddduyl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jnfnqlmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpwwqmhl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2wwlkmelv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qamklcoa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2saiaufgt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tvhuyvqf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2allpawkc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2joglqmvk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2cwwmypua.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zaepsbjp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xoswzexk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kxubdalr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2itilxzhb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xayrcrgx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mhwhpptj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2invqvxuj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wyzgzwan.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2gkqkxjhy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kfsltwln.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cwqzupvf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bpldwbob.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cztncixv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nwzqqjjw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2beowqzsl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lycufjjw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rhjmvqfa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tezskxfj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xcmfxekx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hhgualjj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbhsqiyh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wbktgjni.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hmyzparb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tonrzfjb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vvlsgjpy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wpkeojmg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2yyzdkfcr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dkcraprm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgademjr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aympsmzn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nmievmgo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mugadyhi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2awledckz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cfuovmoe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ukzpxliu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tbcvdpbl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ululfmnm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dghiqwqp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dhobtstw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wdaujbsx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2iuerexcn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vwunqeay.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmlthgvo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yfsmoudg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lcujldcs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xulncqyy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2teeprtza.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xxjvwfft.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ikjtxgms.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpwxbnhr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwajztny.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qzdjgcld.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wergnpiy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bgdgcfju.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xruzpopt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iszbqkio.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2drfhkgsu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2emvqttte.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zllpcuha.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wrbdyssj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2llbcacwc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sbxxclsf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xyfrwjfh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nihzfisf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gwqpmiix.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2laoqhyfj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rpktzrmi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jlurmuvf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2khbrknjq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbubzmap.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dxskkzez.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtfewoz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ywbvukzn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iendlwyt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2sebauuso.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wjypimme.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnnsaade.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2edmdpjrd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cgqkkasv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ogbghjgt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ignphvmd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wxjhjkwv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdcrycxf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2woiumlac.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2oenbljbn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2cddpmhzz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ftfmuhte.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdbxzyil.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2aukvendm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2blqnhmmc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2llltsiua.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnnijisj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ghwppdvc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xthfhvoi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ubkivuld.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rgcbttiy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2drpgdorb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgcfksn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fscdspdi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2omjquvjj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ghdoffyd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zowjdsdf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dzzxjfqj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mzettxwj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmkiommy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2whbqxvcc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qgqqukle.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bzanzzpm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zoigzoac.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yztwxnkj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ntbsjzum.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ogamnnci.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gaqylzyz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tstmkgpo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iqigjpcq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zrshsveo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkohfxjq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kvszsdqt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zjgoquqn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nqelfrcu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cqlargeb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2egmksgty.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xghmeviv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2incffrmd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tqziapqa.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2slwnrdhz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eyvunveb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emonysxq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zilvhmky.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fitojgth.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2drrhhxes.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fbrvyneq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rsypzsrz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vxlkbaed.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fqvflsrz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vjaoodxm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jhbhlrsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yscbekpn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gwlkakpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxbegzgx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pwaixkbr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qlafmwtb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shycwdxv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2scnvssxy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kgyzhnpa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqoqdjdr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ksvuirjy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2aogklqtu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sbagmybi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzbggxtd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eycscafh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rwuhnhfh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xmuwhktv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lsonfjqk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qnxaxsio.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vuxnwpmb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2kfocdcnd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kmvvdphj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jppgxcti.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdbajeq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2btxtivuc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ropisedv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkfznehg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rhqdywem.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kleukpmw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jucerilj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2joolkzvd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mylyisdq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrpjtioc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hierpppp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmvjzufh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ahuchxbb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ajusjcwi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bachyxqy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvnwuylj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2plekdphs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2prfhnpjz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jgxxustw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rcjiscjh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2peywzwbr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2inuvnokk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2hjsibets.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hzmlarug.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mbujvqdw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rjnxcdlh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wsunaibd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rafmzbsp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2grggvhzo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2winyqdoa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cooaxqbl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gymqqfwc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2crixeife.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2berosfbt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qdeakehz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2acnbyims.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2iiemmvui.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dtenutgm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mhanpgra.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2shtrbvjp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2eulrgqtv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xnofwkhk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyhlffn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kztpziha.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2tkiozbnt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2twvaofkc.html


<!-- 参考信息 -->