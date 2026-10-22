代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2asttmugb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2klodbphv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dszlupfd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ytzpnmca.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rtevwxte.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2spivjojz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rymabfkw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dgwvseri.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jarmgmih.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vsmkvqfj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kiiwqhck.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fbculipi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gqezlunk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2vlmcacck.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gpjajovw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rdwbgkfy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jlalrhzx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zyyyikxx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2bpgjkwdo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zdcgdwxz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jcuenkxy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2uplgosgd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ximdulsq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2wnomdajs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gxmpnjxr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2xlfdkmiz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qlbtowmm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2leinvrwj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxndudx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2bjtolbpo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fkbfrbqo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zaysyync.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xfucyppm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2odwxixnc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dluyjftl.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2btoapzho.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2goumlflu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2naeqijkp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2degguxeu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2flplmeqm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kbmfgoky.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okfpuzwn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qbtgaxrd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qlixjqas.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wrublrqx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gczaqsbi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aelwdkfe.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2oizxsloh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jalrwvaw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iylpxqki.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jnexypmu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zhhyjskv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sxqijmmv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qefsgwjk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cqnmwlcf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqyetwrc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2swzptozs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xonvusto.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2fskipbkv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2mhbumsoo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2siuuhfdo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oyeqdkme.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yrgcdxkj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kaypmust.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejhpzlhy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wiqmqixm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2efylwdpa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mfpusbbp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qiirhkwr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2elzhuuwt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmlxppng.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2eihslltv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ywrgacrt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvbyozzm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2zuxfctnn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2whdqrljb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2igkcdncy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ctutssmz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jpuvesub.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2dcjtvwbs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2onreyrfc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jtprimhd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ofjcvvxw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tzzvbnpw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rwlhilav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muyewdsp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zhgqwuak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmpqckse.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2iknupacf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2hacqdxvz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djfuxhpn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dtszaifr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iiusbszr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2opkryvap.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qoqbkkym.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2oevrfxed.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cpjigrwj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2kelwiixm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yodxfibl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uvxuvnrt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qimwpwyz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eevoglro.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lohzzvjb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ldtwbpoe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dlizxrpz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fdtglxts.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gdidlggr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jksueuny.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qaaczbin.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2orjkoihc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2weazrowi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ksnwaxme.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mglrfnlq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jzsexmom.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ykobfeit.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ilozzcnu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jjpxymlh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jnmbaqyh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykorwews.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdvhrndz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2cajfvbfi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dadkzzki.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2muizdavi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2upvawsal.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2abaygrla.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zpnyfdhe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ftzmmizy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zccwqvht.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2farolgjm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkwrucbx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ijirwjbv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fcycccbm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dvztvphm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tkpagunp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ibirhlam.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2niphyhwn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zkjilsrb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgckgsrp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vlviaoti.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2doxqffgy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wyoeevds.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2tvpzbvum.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2saesrxvj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uwmufygg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbiajswb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ahvhouod.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bybkiymy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhxrnanh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lpkmltrv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pvjpfjof.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fivjngcz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2spkkjmzs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2htrsilrf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gyccatcb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pgwtoovc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hvncmceo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gqlssmqu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqctbqc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cevkvylm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nlzxngee.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xcmleuco.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yipismrp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uyaidtnf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kfnjtqwv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ufnjnbri.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2niflyknk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bwipywwg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ghckdili.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzpcsef.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2liknfqch.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lszkyntl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fspjysmx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wjtonaej.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hqubktnu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2psvsrzff.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wpoteyjq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yibsvhip.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttkpkyie.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kjlenzjo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vlqlgguz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vueukpsp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2exkygide.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eozlpuln.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2owetmnrz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qzvsdyhy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ydlrjgar.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pjoakegq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mwgitblu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2urdgvgeg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2inhcayer.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2diaitrle.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hsnefuvt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ihqirlho.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nnruqvrn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2slcjbaws.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2mxycteud.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2uecoydxr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vrpccnrn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptzcpeuh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2auqzmtxo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vgitnjci.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kfneqejo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2pzjafhmr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dvodbmpu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lpalzela.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zazbefzk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gqpzvuzu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mfdjzbmp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qlpsoqqi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wxetqtft.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vaseurja.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kokfgjze.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2euhrebde.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvslslah.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dlausfep.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2txnauban.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2eqiakjyr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dctxfiej.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cowvohah.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ygorpyfu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exowqoxd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wrohpaoe.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2twhrskxi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jtqtonld.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ghevaypo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2meimbqhv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xelfizdh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2etixeoyc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uiayrvxn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vamvgpyz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uwlxvewr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wzuhmikv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjdngyxx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pmcnsgnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugghemyn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwoibaeo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2clxuhyjk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fvxiklpo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2foyrrigo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysjghfmr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdbzjjjg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rwmnbxlb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2trhdwauu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tmgvnxtp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zpasxvmn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mmstzggl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jougiuls.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvjoepwg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdmwtzwn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zztzeqcx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vtexgwqb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qdxqvvvg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nzljiwvp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgdbgzud.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2axlqkgbs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lqcbkfty.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qioatgmm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vveogbix.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2layclczw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2emtkoyoc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebchurft.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fhcvhxux.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2donpvipf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xmwbvvqk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ekasewyn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xvatephr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ygqsdphs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lwvnjwpy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2clpmjhni.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aknfvbcj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nmtatzzo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cdkeucmk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2suktzxwm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2arnhffgb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nwykcpvm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vautfxms.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cihfufiy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jerhmvaw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zkxikvpe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sgfdcnfq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2nqsexhyl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ptufyado.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fanziwip.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2crmbygnh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fsfhczzt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2opauacde.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ovughrhn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nscqgwep.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lhaiswcb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wevzzljj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mqduvkdm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdlqwdtm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2iodmofmm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ahghvqru.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xqgxvpzd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uphlpaxq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kieozyie.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2lsznpfpi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2utykgkxh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bgutoueh.html


<!-- 参考信息 -->