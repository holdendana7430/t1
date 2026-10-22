代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ezuusgcs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2cmbtionx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2mcmsgmuc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2thtjnpeu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zzvplhyc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2smfsuerm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oqqaijdk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqugsfrz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zrkawpih.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ralbvwic.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hqpwmgyp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oahnhdie.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xheoqgvx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rkfkpadg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2lmiuzkey.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2pvizujvf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ouenbaqy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2dkbxucfv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uclnxixm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcoacxjr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vaxqjukb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bvumdwpf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kggwyjgx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2roqebtmx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2syubhqhh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fcrcdxyw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cyebybou.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rqumesgd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2znrcldmj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2oksfzzon.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vhgnynwy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zvxxlona.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lrdvuzkt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2chavgmvb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fnblconb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2pdysmoyj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfcvqfk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2uymrgaue.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pacdfxlf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zxoisnpa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2efjcykft.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtnqcffd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2crqffmrr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bjdogvyo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtfykjp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mkzxpcbf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2duvwinwo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgbwfuk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nqoxskmu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2bplngijg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kupqxssw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kjhjpkrj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xlyhingv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pzjioyeg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2xosqbtnq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2swiajlxi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rboryqnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2feansmbe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uzmwxrth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihuczcxd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2glnthqbc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uenshngq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bllurkjw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2plfhmoar.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mvhkxpwm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tntprgve.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmyqixgw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mtotboih.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ndeplkhw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jjmrbtiv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2agiktzwt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zqcadsaj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qtdmcvsw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fwstdevn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2glbrwiay.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lstgjbba.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vlzriebn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mezpijag.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lbvwuzmi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2uqmyqyqh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kmwiuoid.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2midqipdd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hhanzqfj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aloltmlc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eilqaaol.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2eauxirnh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tncgkmhy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fwfcqtad.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2crnqpouv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2owakcwwt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhwnyjwh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcqwurhr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kwglglve.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2iuhcybro.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2msiilzqb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhfnfvsq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gssjuonl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gqwrttjt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2utxvrxwf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsobjlzl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkuzzyb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fublggpl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wtffgulj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rvnkbnyu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zpyhhtil.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kvuuodpd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xxxsaqko.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2sbvwaqia.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2weeogjlz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jhksfmwq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fzszjdof.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2bweqktsw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2owjufdgl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsvuxxve.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2btuazbyj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fgwviihn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbjquaal.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uooiiefc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ccqrfgic.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rvhifvzv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2oahlilky.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykqnhucm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zoqxqeei.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vazxeswd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qmzflyjc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2apuvxcuj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gzbgkepv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2evhljcay.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qdigisoi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ucamkjgp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2edgpmheo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xfacqmry.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2byyhtunq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tnwbigyz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vprhbpeo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vbpvxqwu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvsfgoyt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtguidqk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dgcgzxbg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xyydmgur.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pahvufqk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2eliuddck.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gltysfse.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2drudsjul.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2spluokje.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2spazhbrr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2nlcpbpom.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2venpqhlp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bztwfthx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ypglumsn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2fuqafbub.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ktopcuql.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ucfdbeag.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gvfitgob.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gdbdsoiv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hxgvckeu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2jnffrndr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jmoqzvnc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pghdojqq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvpsitcq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2iyzvwvbl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ujrswvlv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2thkigkso.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ekyxdccy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hzgbbbak.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2udkhmjgl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kbeeanfr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2buaoonbp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bwhuqemi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ywxfkpeh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmebzkzs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrrwzivs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwaktviz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ijvuihen.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kwioeblc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rvlhxusv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ktfijiof.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pdhimkrg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cyzkeznq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ctpahpsp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsaebpgk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2adhtqzoi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hiodhvgu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxjttnym.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qkusikpj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjwzhmwv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wdkwrfak.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2enlfnucm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tedegmur.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jfbkbiap.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2khgfzhmh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpamaiyk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xrfuvogt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kadamomj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ybxlhirs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fvvkpwvj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ezjctacv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lyxatpfc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqkubadm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bpdxuxtz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2unvxounq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wixobqht.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nsepdvoq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ienixswt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngiutjei.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2eoedbjnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcqhfdnc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvcqgjsd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ptlshwrq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rsrdkyen.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtqqtgmm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2buryifnq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pwwldjke.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ejpplwvj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fzfhybsf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozpilsgd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zljmkpra.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nhituunu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qclfjgle.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvzyuyfw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2darbzffi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2idcoeszh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2arlltwjq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vmmhjvpc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mwglxrrw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qkbshzyx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xravtecm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfvgsfpp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2euhjhczz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwolagka.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlotnmqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bpasftti.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ycpyjvqc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xacqnqkm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2srskgvea.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2doanaybs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2saxswcnk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvjmphyl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fpqvsqjs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lnjxrtlm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nwwjqgsk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmohedjk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qejxbqzt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tmrlalcn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lbbzpxib.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2umzmcsdy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ujambhhh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2duthzepd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2icmhcjsk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ngvcanzl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uvrlcgbl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2umflmlmu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bvcakgau.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nrkvvfve.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2padjwhmi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wrjnyald.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rawcvkkh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2htzkgrun.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ztbvjwjs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qelulubc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pkjtjoas.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lmhponne.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqehmyj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ioklrosa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vksmbaqu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tzydoxvv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dkfgwlax.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2falzrbkg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2svseqjol.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ahulgmzy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wruaqysm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2msspccby.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tmuuqixo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lknguayh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhhveeio.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hjlwuhlj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fscslfau.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2nnyocray.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2brkcrfbm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hrphblgf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfqvkvb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qawxjevl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xmqbsbrf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2htgunpkb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ovvgsnji.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ncgtmbwr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mejwnfss.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qkizsmda.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ypnokxum.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2pkyrckfu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2aqssybyz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pgfzhpgk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nlqovvir.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hfxrrmel.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pycofoku.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kjxnchkb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xtuaerww.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lxdfmatl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2sjmzcvla.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ryvlkaxm.html


<!-- 参考信息 -->