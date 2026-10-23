代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yqlywjex.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bexdqbas.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tbbpotju.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3irqpeyui.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pqemhres.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cymcbegr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ebbebvbq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tgsivwkn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3svlwcips.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3njjlfvxh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tmpbrbji.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3qeimypns.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ialulcrl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vxrwtjyl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ekfwrtjy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3sxbbsrih.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dvvtffcl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xgnafpaq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fxetiaag.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3uiwnwhwl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3faynuwbb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwwqoqi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpixjdun.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3odjmfsmd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zrtfxawq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rtqyfcif.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bdiopolo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ouqgdike.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3npwnujqe.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3aaahgeiy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ennctgmy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ujyeeljp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ohouehhq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3tkfxzqyr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nnbmgzib.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sijvrjfv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cvdpcqec.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mbifoucd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3imbeskuu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmcaaeao.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uurnpoka.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hifjdabs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3riyrgfmc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhhghqv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rrpswanz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3amtozwuq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gfpabzor.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vimudqlx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxpnhdz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3upmuzhsr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3atqtofdr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3hsjthpio.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hrdtyofs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gxhihmxp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ayvjtfdu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rmhfckvd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3wnhnbqer.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fidxvkjf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ngishhbd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgzcwaqu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3oaqrkdgn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fynqiufw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3uawvmqoo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uvovbqrv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3slwnqaom.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3bhohvbgu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pzwrblth.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3cphzlvzk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qhcwpexw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cvezzlwm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vbvwunfv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ucwrkhdy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xdszzyyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmkdxdgl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3yzvdnois.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypkfyeaa.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qmgesmpr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jtjqneuj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxsajekf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3znxkqskh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nivgrsvf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3znhvuhyf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3erxohxhx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3psvljgxo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ptibvbtl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rfsgclhj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3etowifvp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdwtxby.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3atoszepr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3slvbjnpb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uklqebvd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3brtetaej.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zhrlgjrh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qzrnsuya.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nqlclqzy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vsmsmuff.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hwnnbdye.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3urssfifi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dilykqnk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dkocknbr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xnjqhnnb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hwbtivdc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3clyiedsf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3irwepdkn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fndizlyy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pjnsxauc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cpludjgc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfltzhiu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciyplhga.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nieqwqvw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ymnhizql.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3eukzjryr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pfxgsxaw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vjzlajao.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jabzmxpc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xldbhgeg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3waigsttj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvrjpef.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bjklbhkc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lvqrwslm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nkztqwqa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mcabfprc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jjscvewo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfppipob.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ehhavpbe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3chkuaolm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3egqexsup.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lnrpglgq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mtactrfk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmwnfllg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xxncfxnb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vxmamxrl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhxctual.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpxzvxtd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgoadvvg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3upunoiwl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zzmbmshn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvoifwqi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fbhimncj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3oojpbfga.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kkrxkagk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qmexagse.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zcbnhanh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vkftbwad.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3whpsaulq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3efxbeysc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hdugsdkm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3exdeowmn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ydvmhcea.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xwhwuzzv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3muiltoaz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sncuicso.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bwbllgah.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgdizcxh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iyauvvof.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gisodukp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuuanafl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vybfcddo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dcgcjtbf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eplwdqfl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uyexhpds.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3scbhhwgo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3odedgimn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3isriqkpi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uphxugpr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysungdvc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mpdbjkvm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fdnyogdn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ullhasgr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qqjwczdh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qmkxoqan.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eemssivw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3exllnrpd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hwnsbntj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zrycntos.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3aibzcybg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xtueuymg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ipeqsvwm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xohppwvh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cyjwqgce.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mdjrimai.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vesoyizm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kxxnhxun.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kbbucxhx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fdttgzny.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3likrpuxl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hjhyeekg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3viuitaxw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcygniv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wzwxgscz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tfivhkoy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3urcyuxbt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3awhhrknz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hvpcwbpc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3slablbzl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ppmymlsm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmyhhrff.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kockvyvl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wrsnybld.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3iiyvylry.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fxylqlbh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jfhwdgdq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fupnrako.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mvhctqtm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ypihvrqg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nhssunki.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kiwdizff.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sxshwcxy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oqkqzoqe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jbszkggu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3esnceglx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3chyvzwqm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fkslidox.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxhaiky.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ayimafiq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zijljpoq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3eocrbefm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ukwisuhm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vghbrxps.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3psjtlhpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bifpdeba.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fauqwxqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tatqiqwi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmljfupq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yazqsuuz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tenfnqvx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ugrxmrod.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trwtyvro.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wiguqapl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fuzphuxp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbmrpaam.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdcczkna.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fqkkjxwz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3djkkguor.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jrcsttvn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xmxfvjkb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbvicwhe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3anhrfixd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kzbxsxfp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3penxndxc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxfgdnhl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxzdsydq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yueumviy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ppquxpxj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqcsatuw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcxsamez.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3equlivlt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zalozwlk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bwwyypyh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fhdtizye.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3nbfnjsbn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xuuxibur.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ynyokruf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3otlyatwb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3pcgwxwfp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wpiukpya.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3czotmvjj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ekosdoue.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yjoxunkw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3oxzlijlm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yxwdevbo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ppqifbtv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lzyzzuwk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xnwaadqi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qjwcvwiz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vdfteluf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wditcneb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xosyupab.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lmamukxc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3hfzekaen.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lvrmvqrq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mniehrhd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cewtdxxr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cxddcnum.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3krdmbxiy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mxgexhqk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3skcqkqkn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wjcbjtbg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ulftfxpx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yryfytcq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pftnqxwa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3aeqbrivg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qcqnqitc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3aoydakfq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3fyngegnc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ghiduqcz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zaqtafks.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wdizumzq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wstmymch.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpxulvhv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgzsklyh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pszemfnu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3iwvnzkga.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3yiazkmli.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ygfikqqd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3owcziwdv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wulzuour.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wvzxrcye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lqsfnyvd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fdknhccc.html


<!-- 参考信息 -->