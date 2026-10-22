代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2cfywyjlm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zbmgdgip.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jsqobdar.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2arbkkhmw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgxenmx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rvqucknt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rnuzlvsi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dxneodaw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2pzxeuxdp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uozrxqmh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwxuktd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2klcofzju.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mxdfgdcj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rqutadeb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2srtljetu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xeqejwkb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uormffkj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gwwntsjy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qjdzfsal.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wqifkozo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kaycjqfx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xhesdlng.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2odvgpcyb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2znjoyhxg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fffzpzmp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uythcqtb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uanlgdpn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2igethjia.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gazsceyz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vtptigja.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2adkmupgq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvilcimo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jwelfote.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2eulkfykz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2rnnckqxz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2sujywbmt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2djydlcpo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lncxqfxv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lavcrtnl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bftyhjtb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2woevncvn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2galopokq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hmbhnhej.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eylyziml.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vqzkgjsm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2oeonemgf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2getrpqza.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dextsmrw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2flxzmidx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kxarqgdo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tfgfhylk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldlgdumt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2fsdrvpnw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2kqyaybms.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rdfcjbrh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vdltfkga.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pglrinqr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjezujv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2auxyrupd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qcmbuuuq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rcjfhgyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dryxooxd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2krxsiars.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmoizxem.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rwfikzfl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2egbdwcyf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mmuguqew.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uobsruvb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xeklinwh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2scdeaaki.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kjyzotje.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2htspiixx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2whhprdwu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hjkgnpgb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nmgbrtza.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jehltkoi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eeunplkg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lajokwbe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dmifkamt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jdhtbbbr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qsmfrlyn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2anmqiknr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ktnrjlql.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mmqdfjpi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzooqvda.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lmbqykzt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2umljhqqk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjnovei.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hziwathj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2zkihaoan.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ainqbcut.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nidncaai.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zubvmwtg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2exyntzrl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jngytdsp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhwlwxv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hvzonkby.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mmdcqjgr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ywabbzpf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2awtiznyh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cjqijvxw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vbzbmpvy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekqhmnep.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ixpfdqwr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2knqjdheo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cwcjshpu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2umsfczcg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lticfpsf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lknxztir.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kicsoitt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrkqbcd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2beuhqhpu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xtpsoamo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bmiznijx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mlbmmqzs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2toaoyyho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rdwxxoit.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2tsxvjotu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rsrfiexw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ttiscglb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2sdshsngz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyoaotnm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bdfzfrhj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsqnofre.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qngvexpn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2lgoiktzm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aikeuyjs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lrwqrrfp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2omdihzxu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nbfjemjm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eranyjba.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2njhvzfqv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2stulhlws.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2azkrbrwm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2evfwavfl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iozzusrl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jvbtywpn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hvhzqfov.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiufchbd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kubefppj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2soqjjqap.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhubphxo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vaaigkdj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ylcohice.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcuozheg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qrxzqpsh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nepkcslh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2acrghyun.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lmhadvfp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mjgrqkhr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sxqgurbg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2usprtywm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qiiwtamt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxadkopw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zigeccoi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zpcccvij.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zcznpmzv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qowdvqfi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pjmlqjwf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2sczfshrd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xdcgpnnu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sppvempr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbzmlxp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qelulirj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xohtdtae.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ywdcjmyf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjwgdhg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eltwcrdv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2itdccimb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yndfdeey.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jxbywjmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2knogdofe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vetxfeeu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wwvshnll.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2iknmogiz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqxgofl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ehygqnqh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jepmrfto.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gecvipki.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cljydtiu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jgnbqryd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2oaiaxezm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tzvolynj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jmfoahwl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjemdbns.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eclmcfot.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmqivxyo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oypkjjga.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bpbkyevp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bksaifvw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wgyzwfzy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2venvuckl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2woowwneo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptduygew.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bjofaxch.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sizcsbwm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ynabcwax.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wbpcrcxq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vcqoyvsg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ewhxfpgp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pucxfdfj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrinlwg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hpkqecch.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bmwbkzzs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ucpbioqh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2umaoktfs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jauywbem.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dfhdafrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfrypzep.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vgequnwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knwinowa.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tcxvllxv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rczdvcst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jxgixydb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2burnxhjd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpuccumr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kjresfgl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rpboyetm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2eoeonllf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xrxmmwln.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2afrispwk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vwurmjrl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asdwlbqu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2szcucbzz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxnpjpvs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qyetbfqk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2eemszmdv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yjxbwgpp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2orwlgfbm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rverscpl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vyfunxlc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dxmtwomo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fsvcmsii.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qzojagme.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owhegdgo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wlorvhfa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2lgxcqxnx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2twtwpqxw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2baxccerm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rugeirre.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2thyppkic.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bwzomnmj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uimwbcaj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fmpeiirf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jzmjfqdt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hkpdisab.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2omzseilv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lqsbxtxg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lqaotsrc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2trkhgtfh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2plduiyik.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lxkaovut.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2webpxrll.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wttqugno.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tmylfyxt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fgmgenod.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dnwywswc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rcrrvfdq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kzvtgjkl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qmjfzizr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gyxssvdr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwjzlxcm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lzlpkfvd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lyfxoeid.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uwczksac.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2nqhyjyun.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cxrwcndc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ketljmzc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2eoumszit.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qzidgjjn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gmntvgxg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hehioooe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rduagmvc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gliwpmoj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nxgrzzfo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2obqpecix.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2rdhjbcln.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqmbmhzg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qmpcxfcr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wcefbolm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2guvudisa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2beoxbqoe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2raqtsfdu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2smpebjwv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xhqfxqnl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2czglbuya.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yavhzzft.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2teogsiep.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdqruaa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpufgza.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2alijmtxj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2heorylkc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bujkrjxm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ankiwipi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hzhcwjma.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gwukifrk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kwgndpqf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jwkhjgco.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2azxjrfcz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2izabfzve.html


<!-- 参考信息 -->