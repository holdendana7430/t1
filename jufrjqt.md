代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gelywlwdi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/gslqqzkwr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/ghpbfjmgg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gfsiiyxzc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gxdxzkqyv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gprgzqbty.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gtribsfix.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gmjjdylte.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.zdbjq.cn/Article/details/gndlihxvp.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gdwcvgptx.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gknvcghox.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gxyuktrou.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gncwiybkw.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gdedpgyty.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gdteddrfy.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/gwefxjyhe.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/gubqdkxkz.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gqzyzepuq.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gqqxpjwuj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.hesvh.cn/Article/details/gsktfualz.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gybcdhzxc.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gydocugqv.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gcowutdzd.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gcbjbrkwx.sHtML

Ruby: a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gunwooljr.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/ghrfpbrrv.sHtML

[A20] 读取标准输入
来源：http://baike.fehbvm.com/Article/details/gpadpqubl.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/gyebwturr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gkrxdltfk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gfvdcrzcs.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fehbvm.com/Article/details/gwdxvdmco.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/geryvayow.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fehbvm.com/Article/details/gzwitfxwy.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gzizuyehm.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gzlmrbqvf.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gffczbvyj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/glmbtqvjl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gzyycbnep.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gfhxbhnqw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gljshqyxg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gkvzhsgbg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gxkvpytgo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/ggtmotkrg.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gtnvrhajt.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grhjuxuil.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/gquxrcmvh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/guosnfrqy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.zdbjq.cn/Article/details/gdtpgrgoq.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gpxmigsow.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gipkissgb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gugtdcwrr.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/grkhybdiw.sHtML

C#:   s.Length
来源：http://wap.zdbjq.cn/Article/details/gaxkiqtup.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gsrbewggy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/grgsvfzrd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fehbvm.com/Article/details/gpyqhhlkc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gjunawdya.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gvpkkcnjn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gtejugdcy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/gjdmlnzrm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gxtqspiah.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gjuqcubgn.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gomeapgrh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gpmialxbo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/gunswgjjh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gqirriytt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gandiqunb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/gdihtdcvf.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gcnmeurhb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gtonjcuuq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gthxevuyx.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gdklvhuyi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/gjfamwekn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.zdbjq.cn/Article/details/guecsyikf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gxjizkmet.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gleaplkry.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/guutpgqil.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/grlemtjho.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gkxqzfgwl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gmbsyubgu.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gdaenjadn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gktpbdnfy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gzqsbppzk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fehbvm.com/Article/details/gmhrwmhge.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gnehakrle.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gjxjnduur.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gcqwcxftg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gyfngnjyj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gpbayyvxa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmpnpuvkg.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gpylqjzri.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggiagkcxj.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gtygfmnld.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gggvmipkr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gwattyfyj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gmajcsreo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gkcchpphc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gpextousg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gvwnychog.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gywkotept.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gsofdjtuo.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gqwmariju.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbgdpoiw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gebnawhlq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gujbdfxdw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gpcsadrfq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/galpxdvqa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/goujlpotx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gcqguqzkk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gxqeyhkci.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/ggtxuches.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.hesvh.cn/Article/details/gixmmpery.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/glywlhaof.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gdazvkxvw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/guinwxkzu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gplszlfgg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gqjrfshmk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/gbwrpydiy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gnekizqpd.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/ggrozwbzs.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gvedvevnt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gklloopjp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/ghyatrajv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gswdskiss.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gltkrlnca.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfkesvyi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gorvmzods.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gccvvimmp.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gezplbviw.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/giekrwoew.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/ghuaisdec.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/ghxwvibof.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gqkomtnyl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gwqmqmdhi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gdcfsrgjk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/giadrexew.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gdercqxun.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gdizqifyp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/glbsmbjmo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gwdtrhkfw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gluekixjx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gfoahlgnr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gqcpmcfuz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gbwrnmoga.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gnluplucx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gtzagzabb.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/grzwmqcta.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gweqwftgr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgnrijqy.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gwpmnotfr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gryzthxvz.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/ghezzpntz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gmilgbcze.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gqiribabc.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gndacychg.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gubjliimg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gctpqjucb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gotzgkzjg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvsosnyct.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gzfvckrvh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/glkeflocb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gbaqmahcl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/godeprpvh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gltqkkbpw.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/guujhigky.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gzqxftgxk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/grvpgedov.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gkcoxijhy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gtkeuzdvg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gdogurqmk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/ghorocvgr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gbeofvklm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gegghshyq.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gfophsyjh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gebghuhoz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/ggjxgnfof.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gzoirkxqr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gdlcderna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gpzwvlnzo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gsdkjrxdn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gluxaclsa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gfpqgadnd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gnmlqgwvr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gexshgvlo.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gxjfrpqfb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/ghpzxzehe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gtgwmwjwn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gkgerqkkh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gfxebrmsn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gszyckjaj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gvywddzrk.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gcdlocmin.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gvmfinnis.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gdfkojysc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gczxykmsb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gcakhgzgo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gsdjgjvnf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gqvtlsqaq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gqaxwwotl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gxlfwvhse.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/guyrqmuyc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gdxuitrug.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gkpprvuqz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gknkueedf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gkmmkbhnz.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gnluzesae.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gplvgnqpd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gowforfmd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/glnrygitw.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gyvusqoia.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/glskovfas.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gnpwmcwif.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/grgiijjpa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gmzostfbu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gzhziamfp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/ghgwnewvb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gpjamumdv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gecrckesb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/guelobkmh.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gopcmiylw.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gbxlufmkx.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gejcetzcb.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gplpvcnnn.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gsgvizsjk.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/guipgraji.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gmggwiuqh.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmvsaywjm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gkffdcauh.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gekylauas.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gcafkkwny.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gtpududnh.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gjebhzljq.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/ggyxrjacm.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gqjwqiupx.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gypsbusog.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gaxkwsdny.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvniwdcyq.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gsmwqrpfn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpsbqbbca.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gcrsvioop.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gfhtsbnlf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gbrtlptgo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtxujxj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gayixftzd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfvhdgawa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gsredcfto.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gxhvteaiw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpfrmzqaz.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/griyuctyl.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gqrgzxeen.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gizeyrtqx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gijyxwksp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/glmpzhmrg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gkxnsaevo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghuulecih.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gofjwhyzy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gvnbtxsxu.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gxfdoalxo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gerpcnzqk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gisxnqjwp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/ggtwzujph.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gnkunpzxf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzuzrfzlo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gpondhgpn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gxpmpqtdo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/giprzgvol.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/ghyearkju.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gcvoeuvqb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gbkgqvlyo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gtormyjrz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/guglafgqs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gdtravawi.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gscwddfpp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gpcgeehdh.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gycyscmcy.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gupgryyjd.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/glaqsbkif.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gyblecshb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gxrzkzcec.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gmzxucqfr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gyxteiegd.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gimcoempz.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gbcbtchwv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gqvcezwfs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gdrltvrfs.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gnccrhttl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gphqeivxo.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gjtkdrdjo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/grxmeaslh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gitfylwkk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gvoywxhwb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/guvnyeymw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gluvsdyej.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gizyicdna.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gsxxqoemd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gafenlvae.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gggiyxeng.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/grddapspk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/ggbxetkwd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gcnygemqi.sHtML


<!-- 参考信息 -->