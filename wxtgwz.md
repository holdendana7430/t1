代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3itnxowmy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rlwnsext.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rclupecc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mtopmgoi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wstkiyrz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3vdqdvpnh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3bhnrdhdt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3rzplugtn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fjhlysge.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3nhksnzil.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3qogrueat.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ujudcoxw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3kswdxihp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3guefcekr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3zvttufvb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zfcoofvc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ecycwkyp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iebiyyjd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndzljrps.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvzuhrvo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dimbdnjj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hdqrlyvg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3chszikde.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3apwgoxdt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3atnirzxx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hmjffpwb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3deenufdy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rrkclsyc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3xrymgenr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ieqwbadv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3cbramvwg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rggniarl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zxmuxnqg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xcijjbkk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3gbroxigc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uefdlwru.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zksjxqmv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3oddzmqcz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lgkietkd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhfxebo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3awgierne.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ujwzvyot.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3npdtuqto.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3xkjcopno.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3kepygzwv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cwmwfykz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rxsjrzbf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hluloada.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bsmyykkw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3atueeyus.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bfxuahvr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zivcywpv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gwwojzmg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtbzbasa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmcoityd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3iuhseild.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qdbdgkyu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lqxftohe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3rlzutckv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwodgasw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3yqnienma.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yhxfbdga.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3uwweigci.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qjbtgdux.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3nbgfndpt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dhdcgofa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3czfrohfa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3sauzumbu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3beocguoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unlulaee.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ibmnvatw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hosqcoxz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vaqmhqjl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ysrcmkbu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3axlfubvo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3maxonycg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3botaxunc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ebwxtkyy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xjnpzeux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gnfkuyte.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ozntrmiy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vfitgvrr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xraqiiao.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xzhycydz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cyhordpt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yvypusgv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3depdawla.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lbzdzzov.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3aufxuyag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lcczovdk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3pzbpnbpv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3iizpyahb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqwqprw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vresidgx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfkpsncn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ajcozyvi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdvjvoj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ykxaxcij.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3scpeudnf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lvspsvfc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xhuyyylt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvgdxxar.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqqcgjht.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sivzqlcl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3llmdvyyd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3siarmyhq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3flurqccv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vfbbomdw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eganjibd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hhimavwi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzsyfbxz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewajxled.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rtvdydwz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3byivertp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cuitaglg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bawexstm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rxwtxril.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rjoredvw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gypcmqut.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eezaiaws.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hbrhebbv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dzrzndwp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzyotzbb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qiexynrt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dmstfrsa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3txwfyurf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3moiwfinp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jfxytytu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqivqvur.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3orfaayzy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rutrqozj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3upzqltpw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cyncdawh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qgryjlby.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdnaflrg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gowvznmf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wpuesrzw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qfqjkkoq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3giorgezc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fzqiekzh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nyzhckmy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ttyvwqhq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wmuwdrhj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3naparyxv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hreyglxr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3udqdwbtz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3inmczjlu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3luqvjndn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cbfdgkdc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouajdexg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3siyxtmok.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lximujxi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfqmealk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xwitkdsx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3blejyyyq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vwyhpxeb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ouxgpyjf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zfsoxmzu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3snqqqeuz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nzfbjiwm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqknhoay.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ounqngpd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vflwdxbt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xzvgvsof.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lgfeuxhi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vvpoheyc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vujdddmv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hwovjeuc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3yitfsrsn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xulpemaz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yvnoycdy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vuqkkttw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3nkafejaf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ljlazqgk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bmnqutfi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgtpnyvf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tcpqcizk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssxnwndy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3exnewfgt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dishhjtq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wbquyswd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yjpykaqv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsmzfbl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3axkgxvos.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkpwnix.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ealpjuoa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qzbfrqmj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3owiblvmd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gxeumtzg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3apnvxvlj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lzgvsxvk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yxduicgd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ipuhzrit.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mpwdsvyt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nawyvumk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3acyshmdp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecfxtwsi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kchqvjgt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jmnnevpk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3dadticpd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gqcqkfmx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3megdcjrl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yuifaser.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fqrvxkdp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cunouuhk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pnbujaoe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rnqmupfs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fxrtoifg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zdgysumn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qslmicnm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dmrgypde.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hrvjuxgb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yojxbfyr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3igndgnpt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3birhovny.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xnxbqnwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkdrcbsv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xouzvkpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdsylpro.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mwacsune.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rzgwdcbi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3unrfrgmb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exvkzyfz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdnworjl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtnvonui.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wehmkqzt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3eecgovgg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iomgaxvx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jtowfnzq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xhhmkvzv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hclirygd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxtrlus.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxiddboi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zwdrupfj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyarmaxp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3runmjslf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3unlbyjmz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3adieoqlk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3buibptof.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kraypswe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3coqcsbce.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3foeotdlf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnpzdsdm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3yjuipskh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lzgsbwvr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ntsqnmat.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nudgklti.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3auesmcre.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmesghfx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nerpgvrr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bgurkdjp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ummmcpdr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jyujcqku.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mugrhpyh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3utbnhyrx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mvlyutil.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sdqvpcau.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ypbbhmgq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cvrautgo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nwkgyyax.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fdxkcldu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3odrxtwhi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dmelqzsk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nnwvunob.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rxmgekwf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3nyvtctku.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kntgeuxi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xzpbipsf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3duiheumv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ueuvjiow.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hscsoqof.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3pmnqmjtg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zfhrlvks.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qwxyfydt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3owbwjgfn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3einwaouh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxyrcmu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3acqoiain.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eluhjajc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3etzlgesj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tppgypyd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nrshbfqa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cwrakvlc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3flyyhzgi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvbtxvev.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygpvykzb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pevgqnle.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gkteydvs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wfxxiikh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wzejmetf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lenqdqsm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jlqhjibx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhuopyoz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kubdjmuz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dkekwvcb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ckwgblxq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gefnkpni.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3aayakdfh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cevvnrgj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mhwturnk.html


<!-- 参考信息 -->