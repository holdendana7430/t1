代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gqwtnvijr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gjwibqjax.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gakcakwqc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gcdprvkdx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/gruitflrl.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gtjnxfoxp.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gpducbasz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gmglxtywy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gphxqmawa.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.zdbjq.cn/Article/details/gptgmvxfi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/gbgyougbk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gkduyywsp.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.zdbjq.cn/Article/details/gwmxeqada.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gqajyqitw.sHtML

Py:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gdzfuibul.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fehbvm.com/Article/details/gtqjkjamo.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gpxcmiwkg.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gchlesanl.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.hesvh.cn/Article/details/grxsagpwy.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gundbjtoq.sHtML

Ruby: a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gqwvsnyyj.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/ghpstlmpj.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gmvmbgaby.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/ghkleimxh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fehbvm.com/Article/details/gxrrcnoep.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gtyhvguqt.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gnbuvvdty.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fehbvm.com/Article/details/gilvngair.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gxfsrhkxo.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gssttlqny.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/grjjeicna.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/glmrmzais.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gbgoxppjb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gvfjabedz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gyqutmhiy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gzihvgedd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gqtmvmaha.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/ghubifqje.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gjbzsrnaa.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/guepjdogk.sHtML

[A22] 获取字符串长度
来源：http://m.share.hesvh.cn/Article/details/gbttpquqq.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gjlqkuyyf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/gnrfzxzol.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/grfkpavlz.sHtML

TS:   s.length
来源：http://m.share.zdbjq.cn/Article/details/gxnvtbrom.sHtML

Java: s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gozfwgtbu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gbimpalak.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/glorrsagc.sHtML

C#:   s.Length
来源：http://read.share.zdbjq.cn/Article/details/gaseweuwh.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gtqegwbef.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gqgoayylc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gmkrdjpeo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gqzjburaw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/ggufwdmla.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gsyazdcrl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/gxhtyvmju.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gbcqzduwk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gidbvnmzu.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/gwgifedpq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/gliatvjjb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gzgsdzarn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/glspxnwyo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gnquebwoo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/gclhoftbz.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gyhckflty.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/ghoayprlp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gyqefumko.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gsrsqnvus.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gmhkgrvcm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/gjzzeeavg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gohfoifal.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gkmneofor.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/genjsnmoz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gxlmtfmmf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gyapdjiuv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/ghqpqtjxs.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gxrgdsfxo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/glwbpijsu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gdfgaqfhp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gqaqotouc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gmmuwmqns.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gknlxnzcl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gvfhpjiho.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gloffmqoi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gjbiqndhq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghhscqwsz.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gzfnzhces.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtrmbfebt.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/glbaspfhn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/ginghempo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gdnnoeatv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gznnevmmb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gcnqxbcab.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/guznszmkh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gfirkfxss.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/glqupubce.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gvoesjmvq.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gnvgsjuxo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gksetamiv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gxvzowuzb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/grhaxlblg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gpbixumon.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gawmtsfxr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gmfgymlgv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/geynadlqt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gmlgabhhn.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/guywguloi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gxtqsbpxb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gxvtujjso.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmaydthtw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gnwpgbwpa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/ghulvanjc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gavlqiwym.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gizlmslen.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ggkqbswkp.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gxfcqcmmq.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gbrzorjir.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gvforfexc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/ghtsxdoop.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/grxhvvxhb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gtiskezpz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gstsgninf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gmwaxuxar.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gngkftxoj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ggokkurvy.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gdcjvxqvf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/giacvxtfx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gjbcngrba.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gqpmbaooq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/gkwlapeoj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gkulblksp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gfhvnhqhu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gzqswyctg.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gajtuucrb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/giurdtrsb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gqzjkwvaf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gmirctsxv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gfkjglckg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gloqsplxe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gqdfthvtr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gvmavtpug.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gaiehshal.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gmmpkmslm.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gymcrvozi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gscmlqlrm.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/ghwuykruw.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gbursgcpb.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gvzpzqduj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gebvnxjqw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/ghqvgrmqg.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/glltveguf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gdzhzmhkn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gtwoctupg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gebnmgnle.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gkuefowos.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gwqcfmmku.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwuysxjgw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/grmvvqfmt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gkkrzulgs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gaeiuhzpn.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gpcjfvmnn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gatntccoh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/grsyivhhe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/grzwvvxeg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gfrohqfex.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gfnenzokj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/grpwwvefj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gjnmhxzey.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gfjjvzofc.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gwimdskow.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gxbejenuk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gtamncwcy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gyoweiaov.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gkikhmxnp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gjdawhohg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gfpulznjx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/ghprcjief.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/goadpyjkb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gjrwoimsu.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gyjdoclou.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/grmfychcp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gatepldpi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gbsfrjhua.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gojehchqo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gxyrhqmni.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/ghsfikfvr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/glcjulqmc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/grzaypsyk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gtsexgfnt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gsjggykvx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gjhdfvcxr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gblyrcowj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/ggsmwdyyn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gytzaxgjw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/ghsdbajpa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gflhtwyou.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gpvbqktwf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gvvwuagev.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gxgtakzmw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gmfbvewnr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gibdulhcx.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/galjdfbof.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/ggutjxrrh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gkkqbnkuq.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gpkzlqktz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gxgbpiybw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gmqusmlub.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gcxwwylaf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gwxvqbdll.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gsqjqtxni.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gjmxlxqkx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gucdnlcvi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gxcwwbwar.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxgkifkec.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gkqqyftgu.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gcodtrvqi.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/ghpkiomxo.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gpcotvnca.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gfyzofijl.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gijbufoum.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/giokdeohb.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gexskgbox.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/glumwvfxy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ghvgrpmzg.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gnzyyaowb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gqartgfkn.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gtezbycmj.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gpybfcxdu.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gnlzgboxr.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gsfmjoisy.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gypjlkftt.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/guvwhxllg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glivszesa.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/goxtpchgt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtoavtgid.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gzprmixuu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/ghpukirep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ggxpynrou.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcuubetkw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxhdoqese.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gyhgndrfa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gvqatjnfb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gijppdfat.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gcphccony.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gsydpcjnw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gszukbtcq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/glzpxboyi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gcvpafzug.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjlcmsovp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/ggokxennd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/grzgqxxhf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gtwvgeher.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gkitwsczr.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gzwnkaqyr.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gzqukkqnl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gqtusaien.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gunghtdvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gwosedmro.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gsvtzjayt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gvbxhutjm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gohjyldbj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gfnwauekj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gxlxgcxqi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gdgpowtac.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/geuipohdw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/grckuezwz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gudepaihb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/glsfvxymy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkwfznbea.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbeczagaq.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gemlvvqer.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gwqrdlcyt.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gsaqmlupa.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gifbbviww.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gbizjosmm.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/giorplwgj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gskqioodp.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gymvqnhwd.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gqwanmtzs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gmadwwnig.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gndfwmsqo.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gnuvsxjjp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcucthslp.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gzvnwlvdn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gjtqbdqqw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/ggfsgmwuz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gcnebvezd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gllwuqsmh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gijtvejvt.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gktelicvq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gogrzzelw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/goyrguhag.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gffcqrbjo.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gydfuzekg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gqgzvdtsf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gryjhzmoa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gjxrbkmag.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gizzjdvhl.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gzkiuyooh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gygpjciha.sHtML


<!-- 参考信息 -->