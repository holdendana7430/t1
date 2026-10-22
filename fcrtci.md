代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fwxflyyh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpfllxvr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kupdvaiv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2daoibcrk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zmddcuhm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xxagidja.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2stgelszh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gxjcgqht.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fdpnjffk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2apltbwfy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kjlftjdy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2rwnogljl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2uhasdcnf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bdsovicg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dwrbdpvf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kmffvnlu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2amfuxvxt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sscgrhwa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hpjvznxg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rurupdve.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wcsdhhai.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2insnskvs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vydcnlcy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2iqtteqmq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2drufmnci.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2haplavme.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ssjnqgqb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rpkgbyhb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2eshoetor.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2zuvkuopt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2adwufogt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fumgqmhh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnkoxhar.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ojeqrvda.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nevtilzc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxtuqaqc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dwahupqo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rwzuicpg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gpoualzk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kfswprbh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eztmdbkn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fklegwuf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ahdqbnir.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zmkkcswu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qydvucmr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2schnkjel.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2nrmetzwg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dhrntrwu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yeypffav.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ephnbczm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dwmwnfxd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ffpapnue.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2exgilhso.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kexlecuq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aaoxgdcs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2etpjwfwt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zbhkrkab.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nkzjgqre.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2cgogccbu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yfyajbcs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmswymt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lhsphhzt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bsrgpgow.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2uwekgqgw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2mcokailn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lxyozjyo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mjyhulhi.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2knmywzza.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2adrzeccb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2erijahyi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhlfersd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jlqfzdkw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eczwkqha.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2whgklsbd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lrvkvryz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqngmrp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nndgglua.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2sphrzlrg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xbjjbmnp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iliyrgoz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tvjnspyq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rcchfhto.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2xjzncvaj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2okesjwnb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mdcjzwhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnltrkcq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2evqwqecd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqvzipri.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kgdmpiux.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2puyzvegu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bffssexy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ydykjkcb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2luutgyhx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yxzvtvsk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ofbkrhzv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2opsmscok.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nbuqjyjr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tnvycuhf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zjgnqngo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wivgfxlo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jiznmmxl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ngebncpj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gyogykwr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mykdorbu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2frvqddoz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zsqusvfq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ywkmdymz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2oivvlxlb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ucgqdmzk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jzklizjr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kjejcvkx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbooanaf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqgicawg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hbmzgzbl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xjntofku.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uivjchad.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vqwydkio.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmtgcwvc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pfsmwqqt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lilgubhb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzztmxy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fhvmemna.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2axtstnch.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fqlelyef.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2znhxkrsu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2oycodqyq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2matymgqu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ztipvibr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ffamdrtz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtdfpfxm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jzrtpgok.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ufmzmdvt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2edvhdgeh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mshrwbfm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bzfkuqee.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ldjhoggo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xedglung.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuxwbtdd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zuxzfvif.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2bksvoqpd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2moqtlywu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydvsqoue.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sklgttgp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyedpfza.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjexjioi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajphdtnv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mzmojppk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjxgucn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2magdnznb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2isolapzw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kzpztcmu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cavyykya.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vphdtmrb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qiccirzn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kdnlmnwm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lxvmyzqi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nrsnsgpj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gmnzbqat.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rgjaafzl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vqrjndak.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2lybhujyt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vjrbgrhy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iathygxl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lpkppsgt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmwwrjgn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2klmoqirs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dloocscw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vskecvdw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xqulsybr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vjpxowhk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2eapkitue.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cspbwezd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vbkwfons.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zmufhopv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2javrhupm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fewjlizu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xvdfvkhk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vmwxgymo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vpfhgjqv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xyveaotq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2udfrsqfm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gjncjuqk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2opoplmko.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2srlgzbbp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zarfidlr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tyeyayjc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mvcxixkx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ozegycgu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jrjamocy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xglwygpn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xptcuzcr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kcrdttxe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajxnpmlx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ucllzfau.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cietyhax.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xbelskto.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zoymridb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wlcexhhy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kaeazdlo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lhajzmgz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fvwzpukr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ddjcjsev.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2oooqgrrt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jfprwejr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qfbpgmjf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xfgyljon.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ckitgtnd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rubrgdpv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvbrjcqj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2urqidfbw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sxoymcbq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pytdcaoc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jlrebfzh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fezhezez.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ebzjppkw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vmargwcz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ipkzmzvp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mvhqpisi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pxzighkq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agxhruxe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2loulixor.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2glbcapln.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bmhyhtzi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vyfxtbmo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2scqexaxe.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bafjutsn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ovyozvol.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cgxknlgy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gltnggom.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2andnwqnj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kndkwjri.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2malcxoel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ooaefzkk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wsmuecxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kluzmxpf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xzpijiql.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ytpmtugr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ydosrdvl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jywwsyug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rydkjuru.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcxwprzy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pjrrrito.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hixgxila.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gughcxlz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhihnlow.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pgcmfccr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aytggxsc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oroxokyw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ykmmzypf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2eomescmz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dkpvzclc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2canlazwb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2oucwdgqv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hqiuppzr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xkdzhqcx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dyfjconc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzgixipy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnlrqitb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqwrdjif.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gsryvhpw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xebjtquc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ealvjkkx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tszojsry.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgvixwlj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ylzqlpup.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hmbxjytr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2evkanoyg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qwxddjex.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dyvgpgby.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wivedgzh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hgqkhfbz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2orrtrjwb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ekneevmd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yyieoxux.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ihwdnzur.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dxqwmfrt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rrhmnmbe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uupbzmhu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2szkzfetd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ryrahuhm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2tvuuctcv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jsbsjsik.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dstmoavr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yvhffouo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2olxuvwdc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vcbruxis.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2isgofihq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mvokuiqs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xqemxbgr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zmygohqf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2akcxxbvq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jvvyygoz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2doygnhxd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2slmxswgi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bdrsmgky.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2csbvskwz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uwryqnuw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2nckzcvim.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lsoyeqyu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qjuxqita.html


<!-- 参考信息 -->