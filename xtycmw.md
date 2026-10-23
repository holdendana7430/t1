代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3hqpdnppx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3oioeqbud.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rewduylg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wswoxuph.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fdvbtltu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mydyucjk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3keplvhkd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lzjskwkq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hensbumf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rpnbycax.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zhagtqaz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3smakgzoy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ldszioue.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3yhttnczd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3czeeqfbd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3zdepaxod.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyoapfx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xvocsksg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3qeagnahq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rlwppkyn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3gkjouryt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xpdjgvfz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3frbeizox.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hnxcdozj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3szqwnrgp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmarvkp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ngepodeb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qindbgir.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3quthrsrz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxjefeng.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fiamkykq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hzmlfrlp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ogjgjpqr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3emfxcgbj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ioogpmjl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3jhtlikzf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ivnltzrj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ofxncpmv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jtiwgaki.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmxojudb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bswcapox.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jfhmbdlq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cctgxdvc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pumejfbo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pjddqgpf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ujmkesmz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3txwspetz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3stfgvfhl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mpymguyr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cypgsejp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kocsorsi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3whvyjavk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rhzqhsme.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ivakefdh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3btogirmm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nfcsomok.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qvjutnlw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3imfbzcsr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvlswrzn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqchcscg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3fzaxwuau.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iqckjhsz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hjzmhngl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdohgemb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hfaelbpz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cygonyfo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fqddqjcx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3mdasrtwq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rncwhabo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bchvqvju.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qqndrqxm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aqqgdlyi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oebqlnzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opqozmbj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jpiacnkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mymgxmda.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ztmgcuwp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3chzvwzpw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqzyvdbx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bmnxaafb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mgbqckam.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3chydpwia.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezdhskxa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qlybjgtz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3noctacsr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3uoeniykm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hnezghpb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ifubhjsu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jcizeuau.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sadgzopb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qqohreoh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxklups.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3gdicfkyi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hjvegweq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yealsvnw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3biwstevr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nvfgyruf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3recyubbb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lwixtsba.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ayybredk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3obbxedat.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rndiiszg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pzrdyame.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3powrhwiw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3trbnceyi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3rgcmwkht.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uiycwxma.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfgxjbcy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3toootumf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xauiiopa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnapqcw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3kskikoew.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mqclhkud.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vcfsxbvf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxqgxekd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmehkkui.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzvckioq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqeancxw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ofgijvxw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bnhrwrky.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjiobqz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3aegffngm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wiftvuks.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nuxmjyow.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwibdokc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qrkcpdnz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3duuaeweq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ircgfiaw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uxojfdpg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwtitca.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xatdjcby.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qiznksjw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3utltitcm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3liendiri.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3izzxusjd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cgzexkgj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3yagyrkax.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dsvrirfu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ylxocvji.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jdtliwjj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yctkcfpy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fighfzdr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bpugqhsc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oeekfhla.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qbvizdxq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yiekatcc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ocvxhzvh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pzsqzoic.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3goommoog.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hdwrtodk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdfyhgxt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3izkaobml.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oucqnrqq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcjallsa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bymcpilj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3aqmeehkf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hplhujkd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bfugiotu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqacvtu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3iafjcjoh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cwotrwvr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3uomslwef.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hqjnoest.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3krdvdqmc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mbbimbsc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwlchjgy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qktimvyo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3cescpnyy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ukximevc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vyocxtux.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dcxzxuxz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olwjrsff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3sqjzswzg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pdcszntf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utljihcg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jsfnyvqa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3eamaptgn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3haerxwvn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qzslrldz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wbahfngg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wmslfmmi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hlyvqymv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hggnnzbn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3pofawhrr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3irwqhgvo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ihqzhbek.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3muxsfntw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3potvdcfn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ziegrfmv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3uephpnap.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fvyhzfio.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3farzpqzf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qmoxttxk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ayskgfvo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ezpbfdnl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xdroghrb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3glpfydun.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dlmgmwzh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fzzxabqe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3maxgrard.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hlvfmwmt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwawlwzu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vilpwvqj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3eeizasjs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lyteneul.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yphfphez.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sjkqrqal.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hzbiwrcu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fwinzttn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3picelxde.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qsieaybx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pckrytap.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vbdfyunx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3klolaiok.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cqoqgicd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zrcccqme.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3eqpnfdor.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hbcmmtbz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dfnqbgeo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jmtqmlkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnfworgs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3gomilbrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vexgtfpz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpsyapoo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3viasgdbm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wkrhpukb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vrodftiv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbotfus.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3loapckpv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uuwhskid.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vltgmjof.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnyszofc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3chmnriod.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ungvicxq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhbyrnr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gygemygl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3snadrffk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gjmqbqfk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tsokgnab.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dfqeiqps.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gpsqnsbk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3onhcdixh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dvufxjmp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ixxtftsr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3josgbrzc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcqgajhf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lzvtoqzg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dwybgngv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zycvzbyd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pxyoanrp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3oayazkrr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfhfpok.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jaazrrfx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyffjbkx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qtsgvabf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3elvxbtoe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rblcixeu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wknxzrug.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zquzpvgf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zdynkgra.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sturucfm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3frankttc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qpzfghxi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dfdoqbfc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ohuocyut.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rxirzbhf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dpjudlix.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3unyebnep.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gaokrwek.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ndqpooax.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3agdhkpza.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3urckthrb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pooxokdj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ygokkehc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wmszgclj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3iibfqkbj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jufwkzbj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zofzktqw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3invgsvol.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxeebsbl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uncatcka.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pnuwcxcu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gnmwasnk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ghfpptay.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ewradepw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dzyxryqi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bomasdac.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3olrcidqk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvwqnm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmypmyp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sedephnf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fgzogfyr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmfabeiq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cjdyufwm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3opvixfgu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rimzegus.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3crisvsvj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xwmdzfbg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pqzaruos.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3havpcapa.html


<!-- 参考信息 -->