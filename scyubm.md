代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nuimsaqu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcihjtrj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdsjzaaz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wqbondcq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3sytdmthh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pwaiorki.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zllhfcmu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gadptoon.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yupvoksi.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3fpnxdnma.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3odtzrssc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wyksuhzv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3krvdzfvx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mybtejxt.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3omhlbhuu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bocuspkq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wrccouxz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ohsglajk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3oyfrbjev.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nlfdrmgf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dtlekmrb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kinojiqn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3clgeiqwh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kyycchej.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3edacvkoe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qedjbbpe.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3chojoopk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3veragtzw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdsmmtw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wmzcoyfd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3khqgnmah.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3mvuxcqpo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifpivxgs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mgeonred.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzpjaxwh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vfiefbjp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3blgpzcgl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqqhuvj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cgzdszzy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3exsrtape.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lstaxuik.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzzfinmg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zbbkfmxl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3vpemvkts.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cqnyshsm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3wtyhidvo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3izjxegwm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3apdwtqrk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3benwbuvy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xpuxfedk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yzehapwr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjlfnvnt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ajfnrgdg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kxrgyqco.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fwvxygul.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfzuzli.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3imgmufkk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cbxayica.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rbqveiqp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wipxsmar.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgxtimzm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kadkenun.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gxhtifll.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3omkoiyks.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmoywkh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3wwerfqdu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xhzigyqx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffskdmhk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3hnicmqxq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsiewlvb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fizwuqdo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kwnfafrx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfthzhde.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iybmbomh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3glqlwcet.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3atwwwzyg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3liubuyvh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3bogalxgf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3rwykzsbj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qotvaiqf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gkyrzdah.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mfupvidt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tdqwvbck.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qbnxdfzm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3atcovwby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esrkfnuo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3novxganv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wiwxdkcc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3umtmowog.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3kuxdvmzw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krdceiig.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bvojuufi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rzepepxt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3skzavxwh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rxgrxluu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3zcibxail.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ujkvigxz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ynfekhlp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ryzgleez.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gjbycaop.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iowqpdcd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hdxuygox.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pvszojop.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3derpilhk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ugdjhsej.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kzjaugbm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nfipuoja.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ussecvro.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zdcnnprd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jcsrsxmu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vslxodfd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhteptgo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyohmcu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jehidtjb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vittckkg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwixtopv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jffrnkzp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ivfzkgci.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lnomodac.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wklhpdcj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nndtujdl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3avtxdzns.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3igipyzyo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkauapal.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xilvhqec.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qoiuijsg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvhekxba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbupyebm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ecligdkm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rvchpmkd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eznnbqtq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3einevzba.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fifckndd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zdntjzxs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbkfrcr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sagxjabu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rjwdsvnr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lqwosqya.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3iuizfcxi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgxqvnrb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqmndex.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrvhhyth.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ubhbghlw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cxatlubv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoqncsph.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhuwnjeb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3axdpxubx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yosbtijo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tjthgjcm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvecdhoa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3euvahmtq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zmsfptjl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hwsowjyo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ikyllzey.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3snbklwjc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ibcmazok.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nqicggzq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrhiphyj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wnttrzdc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwcvqda.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3pbnxgawl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3oyysvmns.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjwrtzjp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueckxchx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zndvhmnw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3opssondv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qkaujqcf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qxadzszo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3volrsglu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jvyapllp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nfniwtwd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vkfaxkei.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3slaqsqbi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sgcphemy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcfelblm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsufwot.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yidsxtvy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeigomni.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ejfipujz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3siugvpns.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3sggvejfz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iwhvcfxo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ldijclzo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cjogtntt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fzgilegq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3efbsxxpc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3huvklipc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3snqoynmc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3arsokmsf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3huzuducr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zwbqawqk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kglseujo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xcghwjkg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxwxvudu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3scodimyf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hdinlpfp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3inpogscv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3afgpbpjc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fafuwzrh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iyqxexge.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vpihbwyw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qcllzuxy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mepehmsb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dqatjsjh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3uqbhkove.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jimlihco.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mmszbrhq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3upzbhjjb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfzpnwdg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hvsvjlre.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ylvytfiq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kgjuzhgm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eywmkosn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqgiazr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3axnzyrhf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vokjaaxn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zwvlhjos.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uwuzbtmx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3drgvepgc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rcuepnrr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lphjprib.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3diojstoq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ldthwcea.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pavdjwtx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3iygnlqbe.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3iphsrlpu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dpbppsnm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ymqaiccv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wbqprhwy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3eplurtgt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fvzjixti.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tfnqmioy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oovbgprq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3guoywqtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnwxsjhi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3btnhrbqk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hyswcecz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmykrvrz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaamesxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgwqarqv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qezulrxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbrxawvb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ujgezqml.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hztiesoi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3texvvgsu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ktkzillr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fpwjglui.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3irojroty.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkshfhal.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wqanycfm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3deylzifz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3jstsjuvg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hjtsvtvw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3idtnvrot.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nfkorsep.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cbjiytly.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rldldpdp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zivjnuue.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hykxssly.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zpvhlvsv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3aqxlpqli.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3feqakqlf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qglxkvzk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyklwpyl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eiohxhkt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tqmrbszp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ciebxwvn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3prwlurzn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xcenjeex.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lapqgprp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mibzzony.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hbohqpfi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dcewhwdz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3armowcxv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nenyuhtl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kdkdewjb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3japvmjef.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oijzeaib.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aqokxkmm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tlscjrcz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mmjxidgw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uthdxvqv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3eapecmku.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3frmcsqkm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wlyzfkkr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dqixgkoi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3svjvnrln.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oimievcb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wpqrelaq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3akbjwhkk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3alfuaelz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3blllyust.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hkrvrhcu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3emajjrfl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bsgbjmlt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rqkzgvch.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3soxfeqox.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ognlqcys.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ppljxdrq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xdwkhlzq.html


<!-- 参考信息 -->