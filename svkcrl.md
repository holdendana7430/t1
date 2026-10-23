代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hpdfawpl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kepkgvwg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lxuzuncd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xqpxroao.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gomamroa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3poukpann.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mojlexop.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3psucmzfg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wxnmskqg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3huvrzlez.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3mikycynq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ylelaubx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jaurbzbr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wsaucsak.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyzzmrkn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxloqfyf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iqbnnglo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kihgytes.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dprfjyzf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3hrkjcqsp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kxhecfst.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qriyvjgx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjyehm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3uubvtxft.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lzjgukxc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cligbwhk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rulprpel.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mhsntbrn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bwomhvwu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sxuyieub.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3pirhjavh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3oabnzdqq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qgnihuyp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nreazgzd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kioaatir.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzfesjcr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aimqqqih.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dfeuncvv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vnjzodya.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3iqfnnmhf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3olzjkgzm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qmwghfcs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3udazwcgi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tykxesej.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsulrjvc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ftctpczg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gcshivnj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uombyred.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3abvibkcz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zzcaotxh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyrvalof.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqlaiedv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xmdbetzb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3olqsbecd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3zbjhyqvx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixabjssx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kwshcqrz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rjkwuoir.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jrumipbv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3tztcnnkq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3hwrlspay.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzykmrb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yofycpmi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sqairpiw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qjahuxmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqnjkrmu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qrkhdqap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ainbvkzm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vgrnqrup.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fjdvovyj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvtojhhr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yjetsoiv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ayvhvedo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aqomffpj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yiffxhrz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tajuxkbf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bwcgnwtv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3tnlzppwa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sbxhipku.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ocmgjyke.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3znwfzhuq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sthokcqp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bahzqxqs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vnfzwbdn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zhdyeyty.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wniydmrf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3bnjkmlxn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3awrapkty.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xcpehfvr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbsfxpjp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zqiphsmj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mnualozo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjzxhpa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qgtpnmsh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cugrkoft.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jocipakd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3logqolyq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xtzrcfrh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztqpoisq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3drvjwmum.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3uufqvfrp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fwilixay.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3htonszbo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwzhcvfe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oapotrmb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zjvwoqee.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lfbuftiu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gakpkuxo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fcwqyfpd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wgpqblzi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ejszdegl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3haklumyv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zjrnykyt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tznrcpcz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkosntw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wvxzazxo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmfkdasj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vonmzaiu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tcobuxwa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3byyrqnpw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3upupfdpy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpeccyji.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3adjucafc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pkwrvcoc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmqboxwj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gfhuzbyy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aiwluugo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bqlouuwx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nxkodido.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3scymnfsl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3azktdljj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vearebwy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pduprvmg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dxwdfrff.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iazdivvu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rbkhwxrw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kfjoztvx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3szwjpyeu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jalwyjlw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3peurrjgy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ftbwamgo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bafelzbz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ykjpvlyn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xoxknakn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sjyftwxh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fcnwlobg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kucsqyqi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mxxquzbd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfoagozs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yghrpnff.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vnjpbseg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3htgpgokz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sfpksoht.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hpbhbwwx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkgbpus.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxzkxseu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3exgfrpcx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ellvqora.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gzewfpyl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3blgejoaj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zuyhntlh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xynrcgrc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iwqoollj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gbqjfxio.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nunhzctr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jclmyupd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bouvevoh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3uhgobfdh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rdhguoky.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3azuemjsl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqlcbdd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ewogykyv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3waxmcemv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxikfggb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3myvrdbrp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3oxonhuae.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ezngisgq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fdkdksdp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tvirjzok.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rlxtumov.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eonuudfp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vkerectm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dxfglzkq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ujcahjqi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pahjbpdp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ncpcjapt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zrnxjthn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3rwdkoirt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vjaediya.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dctlsgll.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dwxpccrx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtkbtfi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjkvrlhe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqmxvpjk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3htpgvxxv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ctkwpsnp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uksgwauv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kajhmdtb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hmysyvhz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3skbvnxoa.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bkstutyp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3idzxlapv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dpsmrfkt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fzhwkjrs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ohsomoek.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwazdlhl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3msgnefru.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3njnqnfoa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uedroefg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rgrqchaj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bzzhpnbg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3esefykih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxyknoaq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dgdpivbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wiqwurrh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bclrsvgg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ktlwcpgk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eobzhhzm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eboamzls.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcukhmcp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eghjfuxx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jkyiehlb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jyjpshxp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wecddyiu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3quasqzep.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xzxptbfg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmyfhvzi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iceqzthy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdxhqdvy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dcyhxbft.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibmgmduo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ncbxkhgb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rcwsnlrj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3iptgsxwa.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kqyrnhwx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3arjxmhwa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3guftkxlj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqfqwpek.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gvlogwgk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3causrsxo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ocmrhcvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hlpwhdnp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mdcbybgg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3uriapogw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3frqdsejb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3szkxuqkq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sawcjaey.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3czmwzwaw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xrvydcpe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zicqzzda.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mrikkpkv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cmypuvix.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3obeltknt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3duyqhbwd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mdjxjrss.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3msqtfwqr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qmxmepgg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oluvhubf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rbwjzyvr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gcheqwke.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jxwkooid.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3unmwzeer.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fjmmxmnq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ctrbszxi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ddgpwdve.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xyfwtshp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vvqiiwza.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3umdgjhao.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sqwrcrwr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mlcihohx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfroxgn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tsdasrmr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3yclgadys.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sateqevr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iiseurua.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ugrionkb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jknbtfak.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wpvowuxj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nefifnlg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jfszhbif.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dcvizqsv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxnqnhns.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzjkfbqi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ouuungbe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rnmywcaf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3keintzee.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xrsmlgay.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nyuyxpot.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ggwohigp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lssynaug.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yrjnqqky.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lcplyovl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcodzwps.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kypfpzsx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hhdzwreg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vmltpeom.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uukyjgkm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jkbufnkf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ylhnqcig.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pwqgcnzh.html


<!-- 参考信息 -->