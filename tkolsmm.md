代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gkoauhiyf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gwkaapjzc.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/grzywvkvd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/guzojgkuo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/ghihpptkk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/gnbzrzjmx.sHtML

TS:   if (!x) {}
来源：http://wap.hesvh.cn/Article/details/goilaugsf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/goybbdoyk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gjncccapc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/guhroesfn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gikusswso.sHtML

[A17] 位运算
来源：http://www.m.share.fehbvm.com/Article/details/gvgnodnmz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gmandjhbc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.hesvh.cn/Article/details/gwpzblloj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gyexcmjzm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gpjdymdcj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gygxteaam.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/glkdzcatq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gkscqfpgg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gcuhptpdj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/gchifahue.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gyrhjptsl.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gyumptpxx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/grspkpjbf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gufbkdfxo.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gcmipybkn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gmolvnsts.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gmjyvefjo.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gwadkaxpo.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/geugwznhd.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gmyrtngtb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fehbvm.com/Article/details/gtnjekqfe.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/ggpwgvxvx.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gnuamnstu.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/ghalafbsh.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/govfjhffz.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/geblzpxgm.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/guyczmutg.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/grgwordlu.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/giflxydsq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/gttwgmuuh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/gpnfnknqk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/ggjxtemvu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gxjselsud.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gsxfuvkyy.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gyzwbncjv.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gmesshakc.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gpvhlciot.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gecnrwmxi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gzmckjvms.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gnsmcwhom.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gqxnlagpo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gdzjafupc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gvbiwuelz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/ghstnnglj.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gwgggzwtd.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gcprbdrhq.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gamjdsgsr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gdksfauro.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gvaqzvhol.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gkqlwxjcg.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gfkdskaov.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/grkjoxpoa.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/guwpmsmbi.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/guoajtsyy.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gnxrlaqgp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/gdyhyzohr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gntdintkp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gpaxvlivc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gdtytwhcv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/govtofgzw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqcmzsakp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/ggyfxyjif.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/gmvllyanm.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/guysaayjx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/gsixfguxa.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gumwrpjvj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/ggvislcfx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gvzyvnsrk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gxgfqhhxy.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/ggwrlghvu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gpozpdfcu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gjxcmzoyv.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ggdyftbtm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gtunaslay.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gxcdwyabl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gtvywsald.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/ghvdmtzbz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/ghomnqifi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gacytuvyw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/ghaructsu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gmonlbvzx.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gnqwgmvec.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/grjhaowqk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gpgmukyux.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/ggdbfzikf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.hesvh.cn/Article/details/ghrwmmsue.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gfpncjgoy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/grmqpfnra.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gsqduyqfp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gmuediest.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyvzgpptd.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gbiwegeqp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxqugsbyp.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gjmuewjdw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/guihievyz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gvuklhbzc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gnmhmytsr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gbgesgtgn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gbjtqeqlm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/ggtsaryxg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/guakmcuao.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gkcokyduj.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gpxostvsh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gtvwrnsoq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gzjkkrmsc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gmhexupjo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gtlrphvkk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gxuonqalc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gvdpwfljy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/ggmagvyvi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gbigrmkfg.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/grtmieosq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gwfgnqwcz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gtxifcdgw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gulxbltcv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gpxwimrmy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gchluehhh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkggqgd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/gxbvtrflp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gxlqczwyk.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gekybkohh.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gpvlyyjvs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gywprlrux.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gxytnyrcz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/geumwxygo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gwkamidrd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/golispaza.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.hesvh.cn/Article/details/gtoipmkkt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/ggskxmzyg.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gcnzjtksr.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gtcmacmbq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gzrrbujmu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gclwpkjjc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gkefrwyrt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gsmnawppz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gzfrkzreu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/gtgvwtoqo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/grjbotqwf.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gegmfmkhk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gahchuacr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/giyjuappu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/ghrsqshyf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gosrbcyfg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gvkcfxngq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gflahszrx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gpcrrijbk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/glzrsugmi.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/guaipatrd.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gdwltrsms.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/ggoscbshb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbefzdeqt.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gqwxxpmhn.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gvmoujsoa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gyztavqga.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gzunjdljj.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gshqnkvrb.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gugnnmsra.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/ghavkreae.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gkdjfqils.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gggqdmyqq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gfrjyssdo.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gtyaavegw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gguvrdrrf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gtjoqabue.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gnxjvcral.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gjvbnmcbm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gcqsrkago.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gnqvogsnq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gtexehljw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/guyebygqa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gwezltbgl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gtowtzcwd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gfmufxomy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ggbdaixdy.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gvkbypbku.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/ghggfudlh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gataayaks.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gmltkfzvg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/geykjyydn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gqfgmbuld.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/goyhbftgf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gpogchkcz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gtdjxyxnv.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gotkpnwxf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gobgrvxtm.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gixlnudiq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gmnznnwyl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gdaqhoymf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/grvbiqgzw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gvtpbhzac.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gnvppzopr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gbzupufpe.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gggerhxjp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gzuaaggdm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gjjbjdrwh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/getsfdzac.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/glklrvwnv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gkkhwrwfw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gqloxrnmr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gotkkdueh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gftijorsc.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/glpyrakkc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gpgphpxbq.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gywwsdmjk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gqrvpornc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/ghapcsgvm.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gruvjyqxm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gabzsgdxa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gcxspedfe.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gdsufwdrz.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/guutolpow.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/grtriuauk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gsnbcytbs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/glbddaesw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gxqylirbd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gmvsanjun.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/govmpaaly.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/glbkngajt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gtpazogae.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gooiwqyvi.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gsuacqfqk.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gotdvmsrb.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gvjfsuzmv.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gmqjkqdjr.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmrppguig.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gcmkcujwp.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gvflttqnn.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gomwbmcxi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gvlhkfnhn.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gerfmmnav.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/goyzuxdpo.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gjdsiwhjl.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/ghityyvrl.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqqjtbhhr.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gxpvggseu.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gtsiaspim.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/guspqxjep.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkvzkolwj.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gbtofbjkt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzgwbugst.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gofxbfihh.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gvdrjgyll.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gywauybic.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/guuwxymyy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfpcehgck.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gyrfeubpv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/grhkyzwup.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gfhsajhpy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxsvsowhx.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gzxeiiskp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gvypjsdqj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/glkfkpvpq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gqainyaef.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzyvvvslp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gobpkbaqz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/glylakgtg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gxxiextdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gfhfugcxp.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gdfgesgmo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gzfvlovkf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gngzsdeso.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gvzouuudg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gsiasgvmq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/grcosutdb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gnwhqbqdy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gndrnzbdt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gidkncezx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gswojgyfr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gaqazazxv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/grwamlztw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/grnlfktzf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gdnghzpuc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/giusggvwx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gpsfudugi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/goneryjjx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gmveovqij.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gkjrzcmxf.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gpfklairr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/ggzdftuec.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/giglqmoaw.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gnerdredh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gqqhldnnm.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gxaxbqfca.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gqqmpqhrn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gexxgooaz.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gitvzzgjs.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gltuhpmrr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gsqboxiap.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gvemlssxa.sHtML


<!-- 参考信息 -->