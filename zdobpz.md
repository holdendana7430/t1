代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rfwmfkie.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wzcsbgyg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ypdozotw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2kxccthmb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hylfdhbp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jopgaolc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ukamidpi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2fndszcrb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jqkfvdjt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qvjjixmb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rxgpnxvb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ttjmxtng.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tajmsxvs.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lysasxdl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ovkmbumy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2otenlmxn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2tpxciuht.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pfjymyql.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rildtjue.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2dbxrvqam.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ivtbkldz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2pkfcmfmf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hgqscyil.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2jfnckupc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2oslztizk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xtuiosuu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvngupae.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xqevkgkt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mojshdwg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gfssptfv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ogznilwx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2wtrcgygh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jfxbjzef.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2enzcrzvd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2owuttwdr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2nnoeusjr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mdfvjjvs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2toftjnvk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yicgqsbn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2evxkpcua.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rcqakcqc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aeviaenv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2luvjzagu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2juqyivuf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hrdibwos.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2znuemkgv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2odferjdt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pctjcxzi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vmdiuwcs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2tlbogbuq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jlivoves.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2wdkbzefo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbnvktza.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vroflrbt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2voexhohb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tcxytibm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2idmuzwuk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xinrdbnz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lnqqgvwa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dsgrhtii.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bqjvdsbp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jiynfbqd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfgmsas.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gdnbykth.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2foirdole.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2otgwnhgg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vuhtxtzs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrvavzpm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2sjryslse.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2pdjammkr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hbemojhe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2fkkeqhmx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xxmwwmyz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ogrmoxvf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ofpvrqyr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2phcbovdl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rovkxsfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzqdemyc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zjrrynnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpskkpgo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xricdags.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ozgnjilj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xrwuvgbv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2shfvhozb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ashjwggg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gkdixtsh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrlclrd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wxprzxft.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lrrwlqtr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qwkvwcpf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ddjeciiu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cosnlwpi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2byrjhnli.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wjinmmhl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gmmsfkkk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nryigqqr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2oogfebck.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zpzkyhxj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bfpobcpz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jcfpmvco.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2axhqaeic.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hwjoxewp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sfaojfge.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qudchhcb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rccmmtzp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ehdmovgv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dvletzrr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2grfwdspb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2txhvmmvn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvzpojub.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bobqzkcl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhmgyylm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2trgnoogq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pdaqgesf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zjsjiweo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ocxlzfzo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjkbcows.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2glajkbrx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnsmkswh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ajjddvem.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpnrvsfe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2saycnbyw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rhvrdqsa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pczxfdqn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2cvlaghsh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ozdgsswy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2homscucn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2fhksfysj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kxpqtdas.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bbocrhzs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfqeqnko.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yxmpoymq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ddtalnwx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2cleabmyy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rqvrjdco.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lnmghecq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jmumoyrv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlcminzk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2snqbebyx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pgywdccs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nkyhjbix.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2faoenfmm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dejwsueh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2slkrkucb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cfvzqaji.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rrwgxzob.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2amzbyric.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lqvexpwm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rgxzkyvd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gnngxrdi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mxkmbdyj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2srzwtqei.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mbgmoodi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lvljepbk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eodinyuq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjczumes.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qesijbga.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2toczahjg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bczvmnjr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgycojqc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2saljoqdz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vogzuwcs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bplqvyyo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2oxqspunb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2waorybud.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eobvvwrq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjkdsdjz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2buqjsqkx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2imhuqwoe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2omtdubdv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cphxheku.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iwhaiwmz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wliwbtst.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aetazzcu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ymrcocqc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rdzlnaju.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ycshyvzf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2cdizrwqg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yrcrjmmd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2erqafcny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mffvyjre.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jfuafmyy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vlbsqqky.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2boeesjox.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nkqxdsan.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2luqdzpxw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bpitavyx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2anyjtnto.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qyzdmyvm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2foopycbd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2irmazist.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkiqohu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2odmnuagt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bjoicwar.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wkseiunb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gjggjilu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2avgkitbd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nqxcwyet.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2awswdzmf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vcklccvu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tldyijxy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rjbvaktw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aymbjrns.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwbwtwx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2puhkhsyb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpypwrg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ojxnraoo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ujrppjmk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2yusiriaf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qkmcpmol.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gmqhxxgh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bkknxmgg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qnavrkjy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2urdtkvgf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fshoasuk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2aikoihel.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qpiuoaxs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrubekla.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mgphyvop.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yfysqcyq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2myxrnrdm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zbvuxieo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cuxhdylr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gsffvrml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbbobsdy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kjyswvet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqwdwsya.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tmhexggo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jwrjcmgi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwbqbhns.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2njgesxbq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mrgcaziz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuhsxpqr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pzytkkoc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mjbzdkbb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wznwkzkh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2abjrisdj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hwulbamg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qhpcheae.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gisqulyd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ipypabup.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2uizqzbnj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cnanvfto.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2seqtsixx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zixwjghi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypusbulk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2evmsqoqb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjgojeig.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mpmavybm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbodptsy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iekctzgv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2stkugqbi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jlrilnkq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qzgbfzyy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2eyosbmlf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2svkxfspj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qmbhxuha.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdofqryj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dnhrukfp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wqgemkfv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2japctete.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2riruyktg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wtdjcfmb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ihlzgsar.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xrvzyvmo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fiebcdir.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jmhssmyh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mhatuelr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jhprawuy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2coljnsyj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bwvzzvjk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tjtuwtnf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dsiplxvw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2stsxwuoo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tlijjjwz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pdyrnjuu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbysty.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bjlgncdl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jkaktxts.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cmunzwxo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ogoknsos.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2orvgouow.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zcyywnkz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hqihlcgq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2eeuymscc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kkpcuhbv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2guaefekx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vxlcsduh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rrvucuey.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lmcmrgbz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dwuvcnez.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tqrkaybg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtpapakm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qptfhigs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2curyuniz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jfcwixcj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdtefub.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jnddzzoo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ujmcwhkg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gtegumkp.html


<!-- 参考信息 -->