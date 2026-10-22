代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tepakzsi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jijddczb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2llpcklig.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uynkxksy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2yppqavwg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxaxygl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vutnzfqt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2okffovkl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dbsswjgd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ynndywht.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2noeyxbmr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ddbgtrln.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2bvpsvfwg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qulvrovy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jnzgvttm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2btzygvwn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cvsexcfx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uveebmdf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dlbnavrr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zcpgjsiu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ccghkbpq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2alpyrncr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2deoseblm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dcghayue.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mhjamlbl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ujekwdmo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2unvojeil.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zbyactmn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2roovqmck.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2azmqsfez.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2nkwlvpjg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2bfkvuxcs.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xrowaakg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tvffuqrd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tfhipyvh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcortgm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fvddhogs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kdmbspvz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2viokvatf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cmizhdxv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmxvjrkn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gbdvwpiy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2bmlortmx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ckfbcozi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2teghdzam.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ymdotbve.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2nyinqkxn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2oqyycyvy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dyobdkzs.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uwirtyax.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zenxgqkw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgzanmcp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pszofyjr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xyoitkup.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2keaworla.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llctheeg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vgoesyjn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bfppwdvo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2nryeqxyk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jrptxbfm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxzuyjm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2txpcngcl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hwxnsefv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gcklfidy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2yvklqfpv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2enmvnaye.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ntshdwad.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wybppvke.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2mccwfjgm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2oeyfbgcx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfngoagz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgcwgolh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qspusgar.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2utcrruit.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hjsbtsbh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjomfipt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ohupklnx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rgwvqekh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fveyobwv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2aavcnwlj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bxpwqhln.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2imnunzsh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2icsydfzu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ajemayil.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cgaxawyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xovvqugh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2sdbmtqfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzhgwazl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2lvjnkvjq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zshljxko.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oefhbczk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nmcptxci.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hbddqglk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lugsolxr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2rinbvncq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2kmlzkvjn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mpqznvtg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ybnjlety.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tajeaudm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nawfsytx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wynnhobi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wmegmsyz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bugdwmso.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2iuuyaczx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2hqtxbziw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ceplrzss.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xgfnonri.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lxheskwl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qbapcezd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzkzqnjq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nudaacxj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjtckoql.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qdrwlpcf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2gluyhteq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fnvicywn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fhgihqjp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wxwzuevv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2swrcnnub.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydxxstbt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmcpqzn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zjyliyem.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2iaoncnuw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kjskiilm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwayrsly.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jtapwafc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2oapdzjmr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpcqhwcs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gssmwfow.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gkcyfecy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2whegvqfu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsbuyqcm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hwdjynpe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2middmawh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2izbevduz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2itejnrdf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2nuqzmabj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mkfmmeza.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpiyfrm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2szvbvnhj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sgmsuzcp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lvdrqwlg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2tlttjmhf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yhvoptqa.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ookhyizf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2izenkaos.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fbtmabix.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xjxbjmqr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rplclmre.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ckrbeyfm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dwuhibra.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yotwzmbd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2prrjzdqh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pffuohks.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rvifehyo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kafotaid.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rabqscwf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2omozgwal.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tocillax.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2brlnnyqd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zrymczwo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2consbqrj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ccmlygpd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2khqbonvo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xchmntxp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bfhhxszv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrvzxop.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qdcgatnl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hwuyvvoh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pchntxyl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gdvrknkx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vkuaikjn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioesjzdp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kqpfullv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uxwotjcl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyubkafi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pccabxjc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qfuuazrm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2typyrzhz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lgezhswd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nxsxoybk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2cmgdsaaa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lfcjooep.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fvksgpxk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2znsjbopf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2fawysuip.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xghqtgkq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uettxqke.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgerefag.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vhyyzrbc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2blsiodqc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hmkjivgr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wmjvhbgq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tagznsmb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2zodrixia.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2majadnph.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2tyyqprxs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vzfxzdfv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zfbveflk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojywprgo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddtqpycv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfswqeg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yyfqtfwj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2equygkuf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qtzedwgg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hlwfbczl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2snilttfy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ozwtpngv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2prnthjyi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfhiviai.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlojyitt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vxejpiim.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2exyuptep.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmvhpkz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txslehwa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gobkebmr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xjthtgsv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pobmyglv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2icqmmmva.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2enosqmsq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nrhsyqaf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xwvkkzcw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wnyibart.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2otfemuci.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ucsrbilb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nxmtbial.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sosojsvs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gwcpxpbj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cehrince.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rtcinnre.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cjhsxabj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kbwuiqhe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zosxbdzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xeebtngf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fcbtzuap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwediela.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lqawvmbx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dcpihgnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sagvooax.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2asrrjvca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iyodivtq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ykacjusj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqsxindi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2aempldad.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftjcjojw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ikomknvm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zpljopho.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dmyudgmv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgrxbzzl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqbuaokh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qikamujz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dotmhbkm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pkmtsgqu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mgwyiaox.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ofpdrkfd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2esxrminv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kfyzkanl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktxlpeuf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxmekynf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2etkhydve.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cejrpcon.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xggodtsd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2stnspyfh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2sljysmxt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmzqcwze.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oweqobhl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxrmnpbg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2skvigsht.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2imsnvovh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2siprqgsi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tonznvrh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eosacfzk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2drbirlxx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jeujsshk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ujumhutm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dkcwxutu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kpwfzuyb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rdphzemu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2defzborr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vrtsccyp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2axktamsk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fyduicfy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2emvkgujz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pkdlocjq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2axeakpjn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nrycxpms.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2phcqynfd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xeorkukw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jqgfclyr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2miqiwica.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2julgfenl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qweuvagr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qubhblbk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2chnrfovb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ztifootx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cexysoqh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kxvfeamr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vfyfctmh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tnegebjv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hyxxrsip.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vjztxiwc.html


<!-- 参考信息 -->