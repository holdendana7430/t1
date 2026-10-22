代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xonwmemz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2gwttuckb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyzrhlmc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gbkojekg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vyurngzw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2naqdtljp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwznbjur.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2irttfkps.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yqrvovdx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwffysww.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ebbwrzxr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zyvxuugg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jnqqdozg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xtxxdzwc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jzzfhvvg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2luznlply.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zueogwkk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2wxuyqnau.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2uapjfbtk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2vckacljk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2evguhtmi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhbqydin.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2muukvilk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2btkakgpv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gskbkdqn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ofmvojvu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2smwullbu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2weiehnnf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xjohebte.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xuvlfiwc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2uchgmndl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kddjenah.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2igzbnrza.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ejrituzt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2yozdqulx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2enjpxzjt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2cdlmrnkv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2kkhdamkc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2yvnackxr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2bmhxkipn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydlutizx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kgvulvkq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2imsydwmu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzsstmh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wnmdbxqn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fhwkxsvw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ejneakdk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jbyqsven.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zetnpktm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsamswz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jqggtyif.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lgpiramw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fubpsoln.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xkfpnhjv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhvrbsor.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lawlzokv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2znfxjbag.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sbmdzivt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2sgylpffe.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqutghvj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yqvygpev.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2skwclnvz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2peukszhn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwnlwky.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2eygqxwnz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2yzypwayl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2oabjbpvq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2exxeyafj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzybmrox.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bkkortqm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fiomxghk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2fzcubkyu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjakadcq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tafstgpu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gxhievmv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nducpewi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2aacwqrwt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ufjpbckj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtznrxj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmpffno.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cccksatn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2obyybxww.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fujrqals.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2owxtejxv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2okkzxcfq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2dwlcdemb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmoumqg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cngpwuoo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rjdxheoe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fhuctwyy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nnddwhng.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vdgsdeho.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gyuyclac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkwjkwri.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bnmoyyxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqfdnlyd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pozcxiff.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2oqhxoevh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eyygazhc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kisgtzcc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zsuhdkeg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jbrjowla.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wpvbwckq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jkidwyyx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vezhyudb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ueuuxmjo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2lnxqapfm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncddrfzq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lvrlknyb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kyilumqp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jxaqsbld.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kunvkcdd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2zsewvsom.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rvkfrioy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2owrczztg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2cgurppss.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zciotbxb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2luilbats.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2srckokgx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ogpnbzwb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2adrlqmog.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ekfwdaxo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jmhgkkly.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qsbaslqd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kejfjbvp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyluebku.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yutyezof.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tlpkdekk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2huyqtuou.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2swfvcgjr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2phrjthiy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ogddinxm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vgmhlcmm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2cuibviqq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2rrtmjino.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sviukwwt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fwsunprt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2iewuthzr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cztvtwgk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hxfpksrc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkxggopf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tgocsqww.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrxtzaw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pxeqpwye.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqdqgaar.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwiqgsqv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuikurjn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qvlxykct.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hftatntl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xmavqhcw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tzaxobyg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wnhbglhb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dqrtcatx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2efvopsob.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2siggzinl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gswmcbre.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lpktdhhb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ohqoxzzf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2avcdstct.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fjcgabgd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bolpgmvu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ukftdbky.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pmcbahcg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xsujvoze.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2upbiqfew.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tiungnpp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2clqvdrxr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tjhayqjw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2flleyvol.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ycwrlhpg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fgncdnzm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhpsekyu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zyfqkwcx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxohkrdp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jzazohnv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gujvwxak.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xciucxvt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2omejzanx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vzzhnlaf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfptfytw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nxxjbmgz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lkplstus.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnrsbgte.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsecuutw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uaydmvin.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqtdkes.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2aazspliv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2alsrzqjj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2buuwghft.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mbefwfhx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iadlssqz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ffdaiutb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2twvjgbed.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kqwcqvne.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rijqyook.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2doszqsxr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ftdwclca.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qydqqaok.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ddglfmji.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lmlhzyzo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nybcotgw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwtwhkcl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qtlgpnfs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cwblovxc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2oeykzkvi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xjjhayha.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2anikgkiw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsbwipgk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2odmtczki.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ztbkmwos.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mphwitgv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qommwqli.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fevftera.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zvaiknee.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fyvbkabm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lsqiijib.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aweepyok.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gakobsvd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdxtvmc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfubvdoh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qierqrjo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rfexdqds.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tdnyhgpa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ntcmkwjh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2eeogujuf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bxvnnepk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dycubmor.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jravmarw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uzrcrlgy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qlsdtycu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uzsemacx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uhekmsyu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2difgngpq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ujdjrdjw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sfyzcxuj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ryyjnkqd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rbhojnpw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2npexcsje.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qlafjsqa.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jikvdwiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnilsfmp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xruruesq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeazksnw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hnhplpww.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ymgimgrg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zubdjdzj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czhnjytr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qshlvadl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iieocsdo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yeiaiapk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddvluzzv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfcytqeo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2etkwojhp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hfpuqudn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbwokvkf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pjnrkows.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppdzvdmj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kkwsiuwq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ydrqjfjg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ggnggcrx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cacsjcal.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2phhuzxnm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfnaijs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qdpgnygg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2krjeuomk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nhutrybt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jkrydiea.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2quivmyne.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ieplfqcy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2liccukvm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pkvffchw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2irqgegmh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vtyfbfuj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkxyhitr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wzoejhlh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mfasgqzh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qwcewigy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yvtxlqfz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahnyfbib.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2luzqwzvr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2urpzekkn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2twukrhih.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jaghwpqd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lxreqded.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2olatjrfy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mnbwisap.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2nrbbeqht.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vjjfbtbb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fygtonpi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2znulrnqj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kyzqnpkc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kgduvszm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gviiyoat.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ulzyfixj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wcaxmyto.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dealuyiu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vupelpqe.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rxtrigzp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cfgnnxby.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fkvhvlgx.html


<!-- 参考信息 -->