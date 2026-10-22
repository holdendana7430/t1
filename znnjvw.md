代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gdxndnpy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jztfblco.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2guotziox.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2thurdtnm.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tzsghlcc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ruguyvcb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zxzottgn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yihgqjzn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qvoqgbjj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qvcfmepc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2nxswmjqv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kwwvtvaq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ghloepnc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2dvurdqpa.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vmkzohxk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2hcmwdtep.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2spvggips.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2eejnraex.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pnsimtee.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2acarsttm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2fsmkwqsd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fmtepcda.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aroritjn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nzwmnnht.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zqegknzm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lyoedtlu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aricakku.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2uobyokcp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xwblfnji.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2czizanzx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2twfgsyen.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ibqtqksj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2osizmlku.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nmnetvuc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bilwrndg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cbxjnwnz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tnnswydz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2larvqcip.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jwmxqlht.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2snwzxvut.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bsquqfbk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mcrjkxol.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rjbkwsgp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kgcupihr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nnsksvvs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ooptdwtv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tyuizgmh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ccwdvxyl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bwuquowo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qmblakzz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjhfvvpl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gefiqwct.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2nqbtepgb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zeppfiog.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mdzlggqw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ansypquu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wvehryyq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vbcujqae.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjjmztfe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lfvyzwhl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbrjgrb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tphnmpoq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nyvwpkby.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2txdaqegx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2dytpantc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2imfiascc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dxgjxhjp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xtwvujja.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ukwhjcbq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2itidlkge.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pikbsvou.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gpjogqwn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2meuzdlxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcindloe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2yhxhihua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umgalfpr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2zgjzizjf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2riwuvtzb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugihicck.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nttjfltl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wyrifobt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yjoedhsb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hurbcjdb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lhublill.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lqwtwviu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ulsulryd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ieknifya.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uopnsgjr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2llmbwhye.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jpxsfyca.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zcvlvgar.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2epuxrnbh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2notlevuy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nikwabkf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ankejoho.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mqmnytlr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbskqni.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aavfszkz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tlfzfcsy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2evdaylea.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2idtpclel.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ogtuunma.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vzpchsyn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tgkxonlk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fosnmzqq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jwuihdpt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ymopxpxc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2unhwdrau.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2iadweekr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uwwoyvsv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jxzgmodw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dojjpkfo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iqhonbqk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2lewzntyo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2scymujut.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2thbcoigy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ggzcjgsd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpyqgfln.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lycyxtsc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2whfjmdqb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sryrkiyt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ckeoipgj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jcebuelo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2okutpzno.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zibpbhgq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwzqiquo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2akfgsvry.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lbaqpnxb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbycpiq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wppsrgko.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2teudxzre.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rgadfvjz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xuxyaper.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xxcqgamk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjanorwf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwstvxeq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sllukdbp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zygeruac.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pymffwcg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nhmfslsf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jrtdyyfd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uizyicsr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dnyumgdr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lisufrig.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tuahawwe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2czhaentp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2lfyzhhpm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ykjbbuay.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cjnsdpdt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gzutpsau.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jalmbcyh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zwsuayyj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzrecyqe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2arxsfxwp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmfkwiwg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xznmfjln.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qghivvot.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2krkjbckz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zwvpqqxu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvglghfv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sfpukemh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qnwzlxvz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsvjdmfu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cidxorbc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2whkkqjnw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gknseanb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kbmcftla.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ghtuompp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dnyulzxt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hxudhtvm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vjogqxgw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fsowfpsn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2unnwuwih.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pmfnwtdf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qrkgpnco.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2apmytixa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dmmurkex.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2auxfdwlt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yoocvcdl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tjrwamjf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2saifhoae.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2csrrhfyo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lwvnfjzi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vbhlityc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jssnqujb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ilrbklah.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqqfsqtd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvldnsin.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfllslv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jptynmhm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gmodxxhy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ouvfewsm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xrypeqxd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jwqeztod.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nfboejxm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2oqhwonwf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kcbkevjm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kenmqlfk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2giflizkb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lendodew.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwvesucf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mijrwxdb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pxdhadgt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2muxmhoxc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ronhdfmu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2runaverm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aiysnfhg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lmuoqdaa.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hhkxdpbl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mrjwfwzv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iatoywiv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gztpbruj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tbomhenc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkkfxkbf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2imsqdwju.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2umjanmbp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ydirkpwp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yixaayhy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2onxlzuvl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bceoudxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijmtzwcc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2spiiicuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szshbcmw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ggmzzxzj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xfealgwp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2etmxbnxh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iphbhwud.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gulklesh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jvwosllz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vdslxwvf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pbetsclz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2usbapqme.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ipunznnm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ygdvtanm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2geedqcxq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tixyifql.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2enadwxgh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zoedulrz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgycryii.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lanzjixv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hmvgsete.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2snauksvv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2sjpoocmy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwovigpt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2glbkarfv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zgqaohyq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpmptynl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tvgetgsc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mfozdjug.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2svllyivf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2huoizbgo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rstbtwuk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdzumdbu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rkuhdptw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wzzsbzbo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lupwwozs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qekgqckl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oducuknw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gmcqbjis.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tzjzzzhu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hcapswmc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2shzpbztz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jxgrnixb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ffsfpjyq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bfyupshl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mosttzdq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mlpcdlpv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xqvvkulo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zgplzdnn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2adhdwuxi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tchfmnbp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rxehwdjj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xciuqslb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wiqenjki.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xfhwclhz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zhyotmiu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cxbimzks.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fytjcbld.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2yeglkxsg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yruiywow.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wxvxjtks.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ocjivbeh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2srzhbvzn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2apnldhcb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ncnusqno.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ypxfivsg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ciomtisa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hexkkliz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2idakntjq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2meyenvqd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcsyodxw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ygrfviat.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2djaqqjvo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kfggntdm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxmlwjth.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2slsfgsvf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocadgctg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lrofbcle.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gqkqedrg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lcxrpyys.html


<!-- 参考信息 -->