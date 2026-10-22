代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bvxmffjb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qdofiolk.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lhxqjula.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2inpkmrhl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rxdahwqk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tokestge.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2omkcopwm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2aovodomt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2xelrzcbt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2jpakjhco.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dlhylcth.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2exymtgxq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qrqdqowx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kbkbichq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dlntkzgt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gjbymiux.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dltxpvfm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2iveoccew.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vdgkhakg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2miveqqhz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2einhearv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jjmlzmrk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hxczklip.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vukutlfh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2tvisudhk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2evyzavls.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vuxwogrv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2iccigeds.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxlnrkck.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hoahiibf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgghquvw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rqiswinm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wjpswhli.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lkymzyfo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2khvelefe.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2enowesje.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2getfbyge.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2yxzxfylw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2cxtqpert.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2osrhbfdm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2iwgnjflt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2euquctme.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jkdyennq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2urdrxprr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rbsnojfr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2febkwvmt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2anvlipzc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zgdseuyw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kothtobb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ifkocnug.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mgswcxsa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xtgfadzs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qywobysi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rjnmjxcs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2wminjaur.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2dlsdogbl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdjftfoy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2svflftyx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ugizjefs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hliwlcfn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kinpeuvo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2vfylnjyb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hofcbguo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vudzwuko.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zfromhek.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2mxsatsxi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rdixqjlt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpuwxmie.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncejrcwi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vqymkzup.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jmfvvoxv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rkjzuggv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ifuiyudt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2iosxiyjm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dbiziesr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cffludyy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2kkbtuhde.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lsulzati.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2wxsvkbab.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2srkiulvi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2axqvcquc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcfneusc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2tnevilqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsqhzonp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2myldxiuu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uacdcmlh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuvrralt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zqawbzyy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wdltobsk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fajrmayn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fhyysamf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tczfdcbg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qyuxhtrp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gafcecdk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vhkanunn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjrixjeg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2afwzjrhb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2igquwosz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lkvjozvt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jduzetfq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2owfaeneb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yxcssjvd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ibdrthhs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bhemwmzq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2llmtsjsm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkiqcuac.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zhjvedag.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmfamzjz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rkitntoi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kcbrblwm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ssbfkhag.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2muysnmci.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cdxprmyr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ivdktnqq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2huytqjfy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2csuxtwol.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ztjzdija.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2iuesutha.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jhggpzko.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwustgxe.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yrgeuhfl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wenoavff.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbogltul.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyiwxwwv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hdsctljh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtqhujhd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wieohjbv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qfbioqop.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkfvqfqr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2lhywfprx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kjkthufx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2nagiiqhe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2izfqgcvk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hoakpaga.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lbdnunru.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2iodwpxoy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wvctvvmw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xdjigxfz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2umsqojcw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zagooqzr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2oksdujgb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rysclpem.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2leenoebe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eswmoohj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zylzjyft.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kyxfeqxp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rasygeft.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ovnzgvjm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2nhycedug.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qfzyicdy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2orcynnni.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vneiuide.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hbtpiexk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qckjajyf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aehybave.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bngjgxiq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2smgajuvi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xkxuacdu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqdimrct.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2peydmccp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqwtqpjf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aikcglka.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dzcedxpi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xypktvlo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xofcscjn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kqcjjgtd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tpfuklaa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkehgsav.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2skmmonfz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2eonurjzc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2eeiywsnp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2oodjydhp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2olnfycgm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2adymijvx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qezlrais.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wmsbzmpy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jgcmqpum.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fxhnqqme.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ftavuziq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aupggwpj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2abjndyli.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bymvoolq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrpjxng.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fphsihao.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2egxkwvix.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mhhlfahm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpgqjzu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wwnyzotl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xuauvlzo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2olqjbzhp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2fygbstyr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lsbviusg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bsbmjzqj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wdbfuyvo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewnqadaw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yvhyhbkc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xawhnmqi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xqdaksol.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xhnsxmof.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rxtjmzms.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gumtqzhf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2stkuphuk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gquawpux.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gaokfcbx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aodjhxzr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gbrowals.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sccvacsc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cegkevrv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ledcxnrl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwenjfyj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pafissxm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fbaavoqx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zrqyroow.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nosfyepu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sukrbuxg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2husdxjqo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gvjftifp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lzzklptp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rtiyowfn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2njkvegfs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qxjotkot.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdzsetuj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yockqgwh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bqshonkk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lfnmkghl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vyzknuxb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2tymjlrjt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uwqdepri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrbrsdmv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qpbpofig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulmurfal.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lodrqgpi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xvavsohs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swjbmrrd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbleaslg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dfgmmhwz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjyvmdwh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2hvrzbnqn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2utmvfaqy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbywlgt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gwckzhsn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hahmkxpf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gbsnuafd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqgkfbrg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phiadmmq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2axbpzthh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cemaidxx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tgypdscv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cpzprqcv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uavsgpvb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mlovxjpa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2aheywxdn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmhyypyx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzygssbg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jlhxulut.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qkqfthnf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipijwdlm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vrcpftfi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iqsbkqzd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rxzyvhgi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2njhfnhsl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwylrelx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lmoepalc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2adonoacr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ceeokjln.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewyuwwgf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2clbavuys.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2sxrhojkf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cuvavyml.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bajyypmf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hddbqpjk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tcdbirxt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pxwkaojz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vzflgzmy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dkontdbr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2atxaisau.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gntxaecg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dfloepbp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ljabwwnw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sfnochbb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yxunbvco.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uftlylqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dmtasjon.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ooypbfyn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lwgnjqdr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zhthigqi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vkrfzcji.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qhldfvlo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cxgvasje.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2lppfqjxd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2onofejcy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dsvwkblb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ytpsssco.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xlntetar.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lpaxintk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gdnwuhog.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwpcoteu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mhyrzolf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mabjglat.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hcslgwqx.html


<!-- 参考信息 -->