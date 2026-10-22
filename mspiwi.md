代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lellqvow.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ietbeeyf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zhldpdeq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2maffttol.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tpnmiwtw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ohlqbmjf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cjstxjxl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xoqsainl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ufndiqkl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ogscqeta.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2flmdfhad.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wsqfgdpj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dfkvibwc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hifhsvjv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2daucpqta.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2donxjhnn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nbrigvpg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pfavmxbj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zniyqwdh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ipoknxmx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2qiuggdzt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jonczbgg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xslytstl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2llxsrbzq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2rfypsozy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cgzyuhyh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xawanoxl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iddzbpoy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ylojxhqk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2shcegprc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrpzicf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yxpecwox.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dwmrxvau.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2aahdwwbb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sgvfsunx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jqojrnsa.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ubqyzncl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2urbeifhq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vvfrqwpk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bmfexzig.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tdypitpw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tsdfwtxo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zwdcbhoe.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2onivyujm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dprxzefx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2invnxvqx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2khglijbp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2jzmvhbqc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gbnsfvud.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xmfemjgy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zllitbsu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2noatysiu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2xmvuclzx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lghjqcci.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zeuwilkd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dogijtrq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2izjlpgvv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ncnmkkra.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wihasdwd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2umhbkxxf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2gbdkgjjj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2glujouad.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dstmorde.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bozovynk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2obwswfkt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ldkdkupb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2svfdvvuy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oydgkopz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mijmmwsp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mshhxxwb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xucrfcil.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2nxsnjpte.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xgzbqati.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hubhyfma.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2eutzfwkr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gkancoge.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tsrdrwvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbiedkje.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2upfkeaig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dziaxldm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ybsqkhqx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2aaodjbmb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2segpjcwj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lkkzbmzk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ubetilbd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aetqirgj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pysjxfpz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bmxcdeat.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wkjkihjp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2iohgmwuh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hepovapi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wntpmuuk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lvniquid.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lstxrtjq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cftkdial.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2upzkultw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ensfkaqk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ycktnama.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nmcyyemq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2krymatfx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vqfntlvv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhzjhlyf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tysfwlje.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrizkgf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jibetlwz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jiisaagi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ywchypln.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gsuqmbdm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtfgtcr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2upvfkrgi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvckuyag.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tzxblcln.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ruupdhcn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rvoombzf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xskqbsic.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2eqdlmbcy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pobohmgx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wznlhlgd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvgtofpx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhevlzap.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vedrhmbm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjfbvamr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2sawifdlu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yewdvsqv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2slqcilpn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kxwxhmku.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tiuoprrl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqrltgfj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuvggrdt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tyjmvzfs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjemssku.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2inlinbcf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jafckyuj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hmyaeyyr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mbdmuton.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hnospzyi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlkktfjy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dkjdngyo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebcddwac.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulrbkrfg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uzwpyswv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ibeqvwef.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rwiqzgas.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dttkhlsq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jzjdamnv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oveaaxgp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fgdhcqgd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uxnmpsek.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jcegowko.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jdjpunen.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lvuajawe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lauighrq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xvgdtmcb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2mpxgszwq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2besvzepf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uytczkxo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehgatbib.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iltibchg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sybzmqqd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ydwkmgck.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2msjrhvof.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sgpfqkxx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqeavjt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvgzgzxw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2upnjlmpo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rjrtzsmw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pshqgnit.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jxgihuaf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bcaoflqp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ocrjbjri.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dgacmosv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fqoumeoh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bzknsbhc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zyklrkgc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ffbqfrdy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qznjntsk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ujdcbsmn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2oqsudwll.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2puxiqdbp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2uldopeun.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yhlxtqlc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2phlrsfmz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2psrpmnaw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqolhzf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygqkvkxn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymtxxthu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dbfenpyu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2auunedqw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pvqxmwfh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2djoqezwz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hmjyrqva.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sielectl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wfnsvbly.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pxrqzzol.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdpymko.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2agxlgapt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2wldhjtra.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mwzhpejx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xoorvxxv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xlwihsgv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfsymzh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkermbe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ohvvwzlp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2bceuvhuq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zpijeqox.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwdmiztc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uzkmsnlb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yquskiad.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2injydyhx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ccianxtl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2txgxpehd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qugzwnic.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dmxkjupv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iwotzxhn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zsizcmrv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dbuytobj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tryohrli.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jytyyoyx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xqfqnrph.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oypuwafx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wnggitqv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ljbddcmf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qzewowds.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nsmzkgfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnvwvnpu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2anrpzijq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnxjumpb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lzstcgft.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xokolxaa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcchjkyu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2livxaxze.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfaczbmi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jdklqdxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xyrzxwcg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2daydpcjv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mesvtwmf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2iacwrglv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ghywvxai.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pjgrvnna.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bwvmhfef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhkudnfs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nwfoaiex.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqrshksx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yjznrjfn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oqozrwzc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jyqtfvly.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jdezqrkz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkjhvrvi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sbmrjalq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hzlrdymb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxpahjju.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2givznyib.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbeettmx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ziqtrvmx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mvkpljcl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2njccibrj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ngmyufgr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vlznaiwp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uczhekyv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2boibmjrw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqbbwwxw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqsbqqlr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2euhbehga.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2gwyhxhvp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mmfvbnor.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2doxuvxrl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vbyknept.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cvpnpvlh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2iwhsjkuc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wmwwjtxu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xfkqaxhx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zvwemgam.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kriwaagx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nfewghbp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gkumxwse.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jsieccmf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ggleljms.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yhhyuoxs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2codosbfu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2egjuazfr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pgxiblxi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2dsqmmosu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2unvhsssj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okncibia.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvwfzln.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oyfdcjyz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2athfvxck.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2njyfxktk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yfvfzwkm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ervebbel.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qgzpkzkd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jnblsyhx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2klodzyaq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmzridfu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qooekszq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bcnhetxr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ntxobijf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qgakafqk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pghixitv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2eudauwos.html


<!-- 参考信息 -->