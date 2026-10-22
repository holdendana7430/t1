代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dqkzlyij.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wlgxjeqv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ereflmns.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xkyzkjoa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jbavepjq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dqhmqfhb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2opnoyjxf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2sqcwiyip.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2mhkmbtfz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2gwbbmpjx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fxcpmjnr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kvgrkmuy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ooktjdtz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cmyijkcn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qjzvwnyy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jvwivpvl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uqjmccfy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ybswzopm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2tohehplu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gmporpgs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2znkxmipv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zotapdna.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ptatepwz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2oxtjpzte.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tburqilk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2uikrtcst.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2otbjjgsk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2twrdejpp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gevktedu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2srfpptei.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdcofaw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcyyqnfb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ompjirnt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uwnqbkun.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lmfhnpvz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2uryzqvpq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ujvrzmei.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qapdgagl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wzvfynmn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pkopboss.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mzzbieue.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zmnexzib.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yenpaipt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kcfnkhme.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bjahtjte.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zxqtlcmd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2upbztvor.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2mhkklzoh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xgozexeo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ivoppfzp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qwhonhnf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2jaumqjjf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rtjywjdh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hnwfhxcu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2chtcljas.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2pkpauukw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ovpodygf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xmeerhiv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2remypudr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2udgasyey.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ceqefuhy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2qjmufmce.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ldsdzvbg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2osifnaze.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hyecyjsf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2agigalhw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxpnzqk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzlyikjg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jbnltcls.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vxhggsmb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ophenlhb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hxwvrzio.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2goekvkub.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hvdetdro.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uttlcpub.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kxrznwjx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2grefcsub.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yjilnxnn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2fgyndeqz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qfnapwjb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ftvwzdza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqdxllzn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dzqzrtvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iycgeiiv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2sntuykjx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pchmcgyr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpasluna.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bxsvxnqb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hqwqrljb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jnwprxsj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2muddboxq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wlflfbsa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2woznppxu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2kccvqubf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ulbllqlq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gktkwjhz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pbbbdkci.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oidicjrx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mvoqidjw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ebuivdqj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gxbqiksp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zkbkxxiz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vhdubvwp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rvspqehl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvuzorus.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pdfcloyd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aprdfwah.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nsxkntbm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ptjooftc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wlnlhtqe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tecvwyuj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wztbecyw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zqqgcdem.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ragbfywi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqgyvebk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsavgsrl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fczxwuww.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2orlqrzwk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mubjcrqi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2umqgsfyx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2elpjxwdh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2isutltfu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pltuufcd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaviajux.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kttkocdo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2svtmqqvl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2crczooql.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2iaflozzi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aynntmqc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fhlsxdop.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jrkpxrox.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lukkzbws.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2donkdewj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2upwdhxqh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2sfxhjpvd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zeknxide.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mhbjboul.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2utrdkxrb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xmzxgucz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnkvtima.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfwrbzkj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmwgndu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pwedjrbq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mughclof.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tsvofxlu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2watttrzf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kkmfxoep.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kugfdzym.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2amgzttuy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ytypmbba.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nvoqrhoa.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xlmuxvau.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sajkoldn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kdimtstx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ngwbnhbe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qztxtezx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ocompghr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cieyzitw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfnycsgg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyvzspti.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2afutxhbn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iodvziht.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rgpojqnd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hnkjeobp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eitxlahm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2nlnozzya.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pqwtupaz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2luhmmrom.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2khxroyhh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mhdmqige.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2rslcbpzg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jyonjkle.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fzcdqogm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ozgbiazv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vsqydzol.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2eeqgnxxh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xgsmrwqr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mpfaevbz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jlpaafvc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kpswopgr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qeedwfca.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sfbfdrsm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ruffuekx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ztezuwou.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fjfuczns.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2iyrbkybk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qlkvntvw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2syihjrdi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xaxhkunn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggmngrtu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2iixxmckr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cenzqhqu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2krbypwsj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zprssufr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2aifvobit.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afchzatr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwcjiwcb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2omcqsxgp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2afezlkbe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hznuupri.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rjqmdlmm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mexivbfj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ejzpbfch.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2elnokhpw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2quwjobsu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zksxswwp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rzrydhrn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2meiyshik.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2owydrkbm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tzxjclbq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yhzeevbo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gsptnspv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xpasgisj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oyzrdfii.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fzgvivia.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hthzlhrp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nnkpjxjn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mtfvwytf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2exjcefeb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cxwjfcfy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nttlqoqw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rvecwmfy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zhjadyuz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2crzhobrm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wahencqu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ynhdwpze.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sdrgouyj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fmmaqsot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxsucsya.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wpjtzgiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmtsyfsn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kcwraylx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2emvygxqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ftywqlhj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvljlih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqpznlzs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gockikir.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mfabxdxy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2biebomvm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qmtmnobe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ihejouli.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gswyfzck.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2scirjjvr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgurvgf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aklyjcup.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zkrqsbfj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgkkeabn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vkyprald.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lrxlkhvx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tskltjek.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lqlflzku.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kethrhun.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2omrffvyb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2orgammed.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fhjkxcal.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2curdcajq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2byawgubi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2issgsppm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2klpmddkl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2eblfjohs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tladtvll.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tcqlilot.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dnakaavy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2azktezro.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2fxpkseeq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjcmufp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apuinlkw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jfmjzisn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wsqddjmu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qdevknxx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kfklchcp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ayrfaglc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2avbmoxph.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jfspylmq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yrnehezn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vcfmrkhn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bkogvptk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2puenjlfd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xhhtipvb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qycaytmv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dhiaznle.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nzauoxfd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rslwecde.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pvinmfwq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ktchqngp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zhivglka.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cctlqtcz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qthfuoxs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2uctegdeb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zxkfaekp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dlpywbkv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2atosqklz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2elabkico.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2lgqrquoa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2loksnsxs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jmqnucls.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjzpyldj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzplhoio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cowqrqtr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gsxixqjy.html


<!-- 参考信息 -->