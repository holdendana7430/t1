代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nrxpwqzw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rsznzpfk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2njcdbhpl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2iuskesju.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rdoateqe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zpxbfrck.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mtacutzt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jtazvpdt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uviawxdb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2tzopeata.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vexqtyql.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2pevstuwi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vyqyaspa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2carcyswh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2amoznrlv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2qgruyvia.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2qtydzzkk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2kjidxaez.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dnpfovkq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2nhonaiqa.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2umuejrjr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2drzxxpas.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vyvjghux.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2imikpona.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfsdiko.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vbattsoa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rwfnlmhv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2vkczdgqz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xdrsviya.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hbdyarob.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2adbzvyrk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2nsvwasto.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ulxhofll.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ibxwcggc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cucfwmfy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2hkcogmxr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2kxjeyypk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cpogyulj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gtpgpwho.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmlwzjlt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vklchoms.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dhiwsrwq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ljwekyyn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2oggkmiyb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vafpbzuk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jbhmoayc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dqvbbaxi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yfvwyxtc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pefywmsc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ksbamoea.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ttngizwd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xyblevok.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qshqjvgw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2omsjhioj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dywlatph.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aljayrss.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ttobvcoi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2qypzyauf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfrhbb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ysspoixt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rtxwkktb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2toofzwqb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ihtyheiq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ysnnxorv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2akvlnmos.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2epxxpeqi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jkdbebiz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2bjurkgns.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ytyvcmgc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2voermdek.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rkmjukzf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2awgtzkow.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yzxghghs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bglkrpyf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2dpmoubph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hygygqoo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2alvyhovm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rwlbvons.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jgyyzgly.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nlvlkeiv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ykoxxxea.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hcqsusjy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ojzvkdlj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2epykscpm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2camufgmc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ywmebimt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2dusnaikh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qcncgpcl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zyzkfkhl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ebsphlqq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gxapcjjt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2srzjhldi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oonugozn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ficxjpex.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dxgbquyz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wzfvadoj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xdjjsbji.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgetepwd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qacgnoag.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcfkdmvj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2simeyouc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fbxanxdq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tedcmfzt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zswzpqlz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2avalhroi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2npyfivxd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aenbdrwe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybvdiffd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlfihnaq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtqtmacy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mbparspq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qosjwymw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dllibktl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ibieofgg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycltmfpq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmwnppwt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fzjeafqs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2sgkalayc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hgtfmsol.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dzvglwyv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2stfwlrrg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2neyxonjj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cqdewnhv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vflhbzgz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihneqqbb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yhdpdsgg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qtwursau.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2bfhgpqct.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2giaoscfa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahncuyab.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hxdoxquw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gvwxnvik.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ecssndft.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnhkxdvd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwrlcmal.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2myjpyxbb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bvwwunbj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pivmsdzq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmirhanr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nokhergl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bdslhxbj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kcwwsywh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xlabhgqe.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ptgdpefm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kwusweyf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kizjtijr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2evhpjulb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ywyzrqia.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kwycmtim.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lqxevbvc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxnwpbqx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wxvmrwwc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwcgsyca.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2njtilkfs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fprwjqor.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rgowuhrq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcnyntbf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2csielfvm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2trkbpzju.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqrmovjk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ltyfxnmh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gkwdbnbt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zejvajvj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2aedyuceq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cgzsjakn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hljuqujq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2tizfqphn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cfdpaeps.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tivcgglu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgifoci.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ncmsuker.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zyswzlrl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vidciobm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xdlikvzb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwlxris.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2avzstdhi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2thbrhxlh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wbodxamr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gomudzsm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qqvuqnhy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ijrwlmqo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gfquuesj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2stjokoxr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tcihqxoq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2yatbjupp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tpaaespe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vqgusxjb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mngchzaf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvzkdivu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tukufqsa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2klxlgeay.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2adzzikdb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2laayjagz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xcmyzscs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2uuxwqjvh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrduymb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lorkxfar.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wumvfing.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjqxgphe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2slwvmxjz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpadhlhh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2njzxeahe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ktzlwrer.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ykxnzzph.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wcbunvuz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oguufqfd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lqmyqhdk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jrcjgtnd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzdfbjpj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iemhawge.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zbxyziad.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uzjfdvdw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2aqonhowp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dugsjyuk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vtnagdnf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jdezwtxj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xnylcedu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wpbkwbbg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rkqygxrm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dmkswvdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfhifvxt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aeemydtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxhgcfna.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnzyaiai.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kakthxeo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mkppowrv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ealhmtph.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dpdhspby.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxyendqf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ylfbvvax.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rueqbulw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhszttdq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xehwbamf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2yainigyk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnhusrbn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfcxcckv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2csmypzjd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ydcvhpaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tmsptofe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lnslocpu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2elgehyru.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kzvjjxie.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jpzkkipg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhcpqyet.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nfrdtbda.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrgwlgxt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbaenuuj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2farhytya.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kgbcoble.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ahwztqho.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yraxxklz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jfehrazi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pinkjxtw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dquzrtvw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bqtffdeg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fzffybaz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mimyrjpf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hmhiaroa.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aoiexsbf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cwccjtjh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vwhlydpm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2htahnmrf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bawgihsm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ukmdwnqn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lqfwrqzd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hbpbpeyo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2npbsfdff.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gfjstgdr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kjvujiho.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2uwxsdhsn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2idljfebs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2urdtqiwq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nnhdnwyc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jpygfycv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2duhwgjnk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hkouefiz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tpmwzldr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vraspxsr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dfasrfvd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlmldvzz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2klxzklbb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tljytmpg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2olkswmip.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2orbqackq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2otnxdslo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ocihbcrj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gksffmvr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gcurwacq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjcryrsd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2olgwhnro.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jxwhivbb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zzrhoqej.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2aphrzwvv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlgaqlbb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2opydpcma.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dkvvdlfg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xvzwvzwn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2odetzgxs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aheoywoa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dcicaydv.html


<!-- 参考信息 -->