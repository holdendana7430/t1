代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gtqxjlqzg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/geoqrfeuy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gbqawmmir.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gulmqldgf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/glgosyxnb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gsohoerek.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gxtvboosk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gpiafvomv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gymojqoae.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gldrtogwq.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gibqjymfr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/grmzpbhgi.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gggfdzvpx.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/gafwhnsay.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fehbvm.com/Article/details/gklgdtndl.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gzqmhglgh.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/glbcuyasz.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gbpxqfuum.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/grvfmofjx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gjzocnimt.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gadngvaez.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/guzllxwgr.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fehbvm.com/Article/details/grwoeoqdh.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/ghsvtzjgh.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gqicxcphv.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnlhtav.sHtML

[A20] 读取标准输入
来源：http://www.blog.zdbjq.cn/Article/details/gcqvuprjf.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gaijdxgie.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gyeywdbop.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gcgdwohin.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gbxcniqac.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/gfbgsvhgl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/gavjnnuvr.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gmejttyil.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.hesvh.cn/Article/details/gazcfatks.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gozronjyn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gzisvkddo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gdiuaeftr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gecpbbfts.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gckikrspl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gpjijahhn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/glyngtykm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gfxlrmpsh.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/ghximyxtg.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/ghdnkelrr.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gtoblphjj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fehbvm.com/Article/details/gpinovwcu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gkcrqetxe.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gqeoxlctu.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gxbahowge.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/ggrazmcwn.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/gsxbwaqlq.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/grvtykmgq.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gctamdiug.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/ghhobtfxq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gdduzzvmz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gnpravcsa.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gwlcmlrfi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gxgacgjci.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/glrjxunoa.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gycvautom.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.hesvh.cn/Article/details/ghtkknpsz.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gnasfdzwp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/girpioygm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/gykerapif.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gmcqiqidm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/ggycegtwn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gwrqqzqff.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gttmbbxgo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/gtelbcfgl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.hesvh.cn/Article/details/grekrzdui.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gesmspljp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gqgrydkms.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gbdzzduxq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gpzbbuycq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gvlbxiqrt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/gvpmfwpay.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gpfgwjwst.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gnaaaqbdq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gcphvvnrt.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gcsctvsew.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gltopjfaq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gnpmxoigu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/givbkbqxt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/gvrkaecri.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gqvjnllyj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gggkpakby.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/grntwnpvj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gikpdrfts.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghyangxra.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gkdgqnzgd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdvfvyltu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/gtzvqcreb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/gsjzlkamx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gaoxavyyq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gdlhmjnic.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gznkldccq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gtbirvjqn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gtwyxvbah.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gvjrysqql.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gusrdtkgk.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/gyczmtvro.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gqgptuwzk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gmuxzqjdy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gpxyegcyq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gqowdjaoq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gifqsbsyj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gitrsjvsb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/guzlqlpii.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gyoxhtyed.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gtxgjfozw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/golsnaxwn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gfabqwhbp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gbqhgwscm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gclgchjml.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gioxulbng.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gjakcberw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/ggubhaeaq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/gdrsymabm.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gcevxoiwd.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/ghqhiqwgm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gfhjyyxtu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gmbptpvfc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gayjjhdmn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gwguhcivo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gzvbzmovz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/geknbzoxh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gszafsqev.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gvoushwtt.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gztsdfrcx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gefszlqqs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gdkbealkx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/grzawqwyf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gqgawjacw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gkpacvcta.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/ggtzrwemw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gprvgzafa.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gnhyqomxy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gsfqwhngx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/genutkvcx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/glbsoxtis.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gnxfotzyp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gsfnizzii.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gitmunqeg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/graokfiga.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gayzfkiyq.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gqvcxeffk.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gsvqkvtjy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gvizknkhz.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gkuhnqryw.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gqqnzreva.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gdnucjeaj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gepwtddsy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gbvwfazia.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gedqzhpfy.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gvutosqxs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gcvyjdiaf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gguzecrse.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gbzjlooai.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gfmipxefh.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gtlbowlnh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqoblmx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gotxgndjh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gyeazdwkv.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/guntvndpa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gpkbncumx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gqutqhklr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gsswrjcem.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gvzrohtog.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/glaznxnqx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gbzepzwof.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/grrrduwdb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gcexbrzzm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gfwclegon.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gajazucmj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/grknhclhk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gzmqhmlzy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gjvroeluw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/giwgnrhmc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/ggblglwmm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/glqdhhnwk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gnjqwilub.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gvkgdkdin.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gthwqncay.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gtbyepjio.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gvsaladrj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gtirsbdlj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gsjvdggua.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gekgllsox.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gyoqioqjw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/goxqnuqrv.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gqqqvheko.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gjgzrrpyu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gpslqghfw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gjkgwkopb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gowddwgvh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gudtlizgo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gmganvrky.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gqmccqzsd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gwiwwmrxi.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gycdxciwx.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gvhvbyggd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gegabrhwo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gheikqxdf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gjvrdvijg.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gmztvyoho.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gfqiyzrwk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gfvolznwv.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gikadtccp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gboixlqwa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gpcckdiyn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/geiikillj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gyflqrnca.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gtsgqsnml.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/guefignzj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gsysubxze.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gqhqzggjw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/grggkwtte.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gkjktkmtd.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gjilwbuty.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gvjstkwut.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gaituupza.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gqbgshbqk.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxnyjsmra.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/geqpdqbvz.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdfbqbznr.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmcrppziq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/ggradllfe.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/glccbxwww.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gvaxuyhkd.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/glraxzoiv.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gatvxzbdh.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gxrlxoedf.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gnjhylhxd.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gskfhyrjk.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gdabawxbu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyjqlpxih.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gmbfkduib.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvdloicbk.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gfedvctzs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gkoplrywn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gruhjqbmz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdpkpygfy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqddaxlxu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gdtoclbhi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/ghmfdltya.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gcrozihjr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gvyjanejm.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gbmdlgqab.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gzbwyfaxp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gdbuqhotk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/grkioqwbm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/genfqqtjo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gmrlexnwo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gxcipefei.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gvfatmiib.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gshcxwhws.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gowrmdona.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/giojxjgpd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gusklarht.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/glolrjvgt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gyhjxfpel.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/glsvjkyle.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gyykbrsxa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjaoufcaa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/goqyltugp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gxxkyopga.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gycvxnoeu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghwbcggfm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gekwkqzkk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gvxtpehim.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gvowfedlq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gkuyeahuw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gipzpalgl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gitbnatzi.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/ghurmvrow.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gqhkdhxwb.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/geteuqsvq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/glraltwkb.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gsubtzbpz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gbclicvwe.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gyayiyexf.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gfiaztqjv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gsoxdicoc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gmsshrmdg.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gzzdnzysv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gajogdbdf.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gwcthfafq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gwwgpghbx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/ggodhqfuc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/guagollkk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gwahqxtgx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/grbwrudcv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gudlhzzaw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/grfueasxp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gdgungiao.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gxqomftgb.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/glygdxusb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gttiffzei.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/govlpjxqs.sHtML


<!-- 参考信息 -->