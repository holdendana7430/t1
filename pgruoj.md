代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bmyibruj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jfwqpggw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vkdsrjsy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hqjzavus.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dqbtlpdh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lrrntybh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3aqmswsmv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3purcrdpr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3imzmxlwl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3txzbzbwn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpmywdkt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvwiiprm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3udttqeum.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3qdqwuwuk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qintadpe.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3nanxxlga.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhmescqq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zzjswfsk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tnxbkclc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gcszzmmx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hknkviku.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qjevmzra.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3szmfjcpd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wqmckrzr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3awxifhnn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jxuwnznm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwbknao.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dpdfryyq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hipztmwf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3fzcbfhkp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rnweplrm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3iqnukesq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3wkghujdx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvxowics.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dkhaxydl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3phonkqbf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nnorvztq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xqeundof.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3gjvboery.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3inelbqtx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ldxuibfi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kcliyljf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ghdthpti.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ogcvxeov.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3tebiwtbc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3nupadvde.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gkmnyrhk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3aujuhgin.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3dvkzydrf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3kpvqdrbm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3qjxnmklj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xoqugnpp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3hdhicqzl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lziifmsq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3huiltkcs.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vlwklubf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yeznnpjw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sluwklvv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kribgqbe.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3brjhxvaw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gzggnprq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3sufrayhz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3tkyrtedm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tafvhqrn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3werrceuy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bdnfdfec.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3odnziwls.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3enzaemoy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3irtyqqkl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ktrqauyc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nlknsdek.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vqyxntvm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zafmipsg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hxgvydna.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kbduvcpq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3plhaizvt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yehzxdkk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3numbvefj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vbqzlthm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tydzcuyh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3pktweiet.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pryhzmno.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pqsqxukn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qqhxtsqx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqxmnewc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3wrhmzetq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3knamaodx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3elhmpjpk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yrpejaei.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lkrcsmwa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wudapjol.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3iszjyoct.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kpgieifa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fgvzyokd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3tbqjtkdm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ustwmrkh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ncwepual.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3civsdyka.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zzmskdfs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3pvhebdym.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3hgkpxgws.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fvdcdnic.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3chymsykc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3agtpqdqe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fzcibzgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilttstmn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zttcfrgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xniswvhf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3dwchjytq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ygdmxqep.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3osgpjinz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3omapdowz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ctrxrois.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eclwqudk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3taxlpkvl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3suduelts.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qmtgkzmc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3somlddcp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dkxxgipe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzhiflpw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ojspialo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yblxekco.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lpjtsbbr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqqfjwqu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3akeliqxm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bgoacioa.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3anbkevdp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3snakgwva.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3glmdylye.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3juwqffjv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdonutpg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hncfdjxd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gtfpkirv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wfsrrnpk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zcceywty.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hntixdez.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ounbzkqy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ngrzpcbd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eyabypec.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wnqzmufr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvfprtkv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pzugetqg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ioijbvhj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3swgymtqv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nheagtsv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ibfnwwyu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3veizdayg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqqgpnce.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sppvoxgv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3yuoeswkv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mvldhgsb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hyedaylj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qljovyei.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3evihzmdo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3azliperb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otysuwuh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxbavia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3julpuass.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wcbjmjvm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3feprpdbi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3brzdsyzf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3eixowznu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ndjtrmze.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hryxturw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cxekizvf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwetdbry.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmrdapk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvalqpvn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wxzdsons.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zttdonyz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnrubffu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fubqqkho.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3suzsxltl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rcjgigyg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mfwkikak.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wiokkjzd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ejbaiupu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ttzocxwc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qwzirher.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lzvrrpic.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ndwwnlhq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qfufbupf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mljdyrwb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wxwsouey.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdvrbsnp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dttkovlv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rgbtnkhc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3uevajbgb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vvustpey.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wtnfoywp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zxwgurfd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3haxmpsph.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mlrkiqtx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ersyrgal.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dqzzpzmq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3isvbaxfx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wszdvlec.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mofmsvor.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xyfambiv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bxkbqbqi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bambocmo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tdvamvat.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oorxeekg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrdxkrem.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3swzrfdkl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3raojozly.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzxlnxzp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xnqikrlw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fzsusipq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nocujgft.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wzegudci.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqatpfc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nwljaype.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3aecuwcan.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gdwrlzfj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ewwpygpz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nduiiyka.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3eghsgssg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yntbckgk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gfvmhyzh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3krhzrtrw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rcgglade.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3osqaigvf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3twwejdhb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ptsefoyv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pblisxjc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3niwxckqs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3mrosfwjs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3igtbwlzq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cojdiwji.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftotepog.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwtnetl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnaushr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pysbeduo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3svwddvws.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xgdoprkx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dkjsegal.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3klrxiegp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rrbjqnkj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hcphznyb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sipnxnko.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vexezmrw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3edastwuy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vdfmmsxl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cgfofuiq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jzausuzl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ubyhyszc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sasxzokf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nahnvbvn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xwjuauxy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zfykqjqf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hqddkkyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brtnfvlf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nogssblj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdrpqmhe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgfuhqya.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iarjgmth.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdeweflq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyyfntp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ryuzenel.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mlnuaoev.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ssmbutav.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3srgiqjqk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3roytzpsg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qflqlede.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pbwctvja.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jzhypzxb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bkibowas.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqgxhxle.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qkyyumyx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxfvzcsh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mojlgrfc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qrtxgrvh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyqusumh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kdriosoy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3humkphrk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3udgzdfen.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziiijjbr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3moeqxuqi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xlevuniy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dewocqas.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3anacxfvz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3absnfprn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3giopsmac.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bulmpvjj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uycwpyue.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3asmodshf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uozdzlsm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3movlojke.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3esyyvehv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zcqpxttr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pjeamqqo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zuvvdogu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vryzqoqy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gstwtmwf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wdlpinlv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3adpiqdtx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eufwbdbv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pgzdtyho.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ilhjvdvv.html


<!-- 参考信息 -->