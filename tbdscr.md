代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3dmsijsva.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3uwyyxxow.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3patuqtjx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttmxkzbv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ouiepqyi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3qswijhfd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsdshtkq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dotwthry.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ixfbtzvt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ituslqlx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bjqureiw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cnuowach.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbhxeazi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mglnotke.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mjbvisjz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfulizqm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xpsmpjyb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oaozyjat.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mksepxty.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rvgqrmsi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gubrhasz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3bndsvtoc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rzrmburv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pqrnrwhm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jmrgazvf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lmlgnrga.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yxdwqbzt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3fvohbcag.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3isueyybs.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hxqjqqva.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3jlibilta.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3codvrktc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wddoossr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3lpwjjiqt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hwctztas.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3bdmnpxwv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3dluzvzlh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vgcttxua.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xklgvoav.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3mgfaovwq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3sppzyujq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3mrnsnjji.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3bmiuuywj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3eomkhubb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ybjwkgrg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3plmyptnm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbfcxhyt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3glonemas.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgsdkmc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wyanaium.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hqonnyyg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jdqbsqbl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ibpercvr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpekuqzx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3meogpffr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hufreqyy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mvhgvfmx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jwyntdxi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3essqeaiq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wtsecjwq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tardsewn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nndhqtgw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eikfalxw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3klxhntmv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aeqfqhcq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rwywyuic.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mqvhqbmp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3drslpfri.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xnrgkarb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tuplionq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tgsjvmla.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xmtkcopg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsqkmsfo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ojtmuwnf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vzocwnee.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3diiwjzow.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbjifhg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3nymxbbhs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vqzlwtma.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yktuwbwt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rgwxvkvp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3olyfrohi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rssrunsc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oqjmutgn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcsujdjh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jpagkdwy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3uxvkaohx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rccoidma.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3cuvoyagk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3uwdlcsed.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kqobfgfj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xgztalwf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ueqnkfvr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zkubxtxt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3apbnfrif.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gwwvgsxa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3axbjqvje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tetktndz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3mtmugqom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwifolwy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vlhehwsr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bftocqkx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vixpnvzp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vedunbek.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lssynats.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3klcnkrrx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ocajmekk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ippkzydl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bicobsof.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ffanvucr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jbqbkgzx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xiygojsn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3meqidtyn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qnaqjisz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rezfcwpf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cxfdyszr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3cdjqrsgp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3desekwjr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3llxejgbz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3utusxwwt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dzatssuz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqmhxsne.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3alpvpwpw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xhmpuuuj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fpzrdvcq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3waombibf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aersnftu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sguazdbt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3sazdwwtk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lqutjfnw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3girlbrhj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyqabwbl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vegvecra.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhgvfyad.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kdimgdzi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hkoethmq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kstslgic.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3luwigpul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypxzaxkm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqucownq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3utpccwvq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mtawxhcd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nicqrpty.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ohcyntfu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ljdfbxgy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vhgfrrom.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pczvalni.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gkmlpcem.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjsryayr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3onyricye.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tbqdwnzz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqgpzwgi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3umaboiyi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gphjginp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gfbgksag.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3miyrtngu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ewvpjaub.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sljsrkoa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ianddqjx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gtpugjyc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3emqhirlf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wogvwkst.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jljkznvi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3thrbuktn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hwhqmudc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uoioszqe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tpfqvouz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3emhqfuyb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gzojsylb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bigatdhw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3pbrtzzof.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eejbnhgx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fbdbavlv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mxowmthl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqssoczl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3whbxnvbk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3elgzphdv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqtbfjiq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3puufgpqm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vezywbsj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qyxprqvy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cvhlgnja.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3egmzzqzb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkzkvzt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tzcqkqgn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3czgefaiv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uehpiyid.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qpnxjcoi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3okcrzgrw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ijwhqrpk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qouczasf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ehbtzzrj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3idzteljb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pyipnmtq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zeupopjj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uexiueyo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bcgnljpq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wsnpqzew.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3slsblpkb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekzvdmmu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cpiqvluv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nqortwep.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ucchyxmq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gazvjmyb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sixgidon.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3puorkwdj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3odpogujh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3cvbwirgv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kylxithz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3onqdnice.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3audxxmyi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3muppimzy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3amkfxpdv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3azujlwie.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3glrufuqh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3caphnrek.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ocdejass.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gjruxeud.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3cryoforh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3bczhzttp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3osjmalkm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzipuxfw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yjzxdzud.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxwkbzxy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjqajat.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnlvvgbi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gvcyrnvc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3upxtpunm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ozeecvbs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oeunydpw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gmnnnzeo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xgwsdfid.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qeifheap.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fkyxhzdh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gubqsqdm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hwzljhmj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tqqiyoyb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ckfajbbz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eaipnvmm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gzhcezvy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3idjcranz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3daxywuvq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3svivmfir.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vnycvqhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbilchdf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uvgqcjnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jawwrqhk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ismcesio.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jiqtrgoj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3orqtjcku.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kxdtttcc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rwunpnfs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlzliwgs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gedetzjc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3myatlxsw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3izowydeu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmdfzpix.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bnwmlytv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjslszua.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilyspuxm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsaxcxae.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vmeiuiro.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pumfykej.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jyamlcsa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vqqirgrb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xvwkeeyy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdeocdi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ewubsxtk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhesourk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdoppchm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3cvhvioye.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kfsezozz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tfcqeqbs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3osnqueyo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pjbesymc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxifdie.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3iywyridq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zvqoujwz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bwtasmbp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gyebbldz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ujwpsblk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fcuhnezn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rldfafbi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yskjlbpx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lxixumdz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bqjhoonf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iawvjmxi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mxlabuif.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dpgaoiqf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fbagohsx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3drjaliij.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zqjuruxx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yvlnemrj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dybsmtha.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ibhxvnou.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rlgdxpwa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3extkzodd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3idizhety.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eoeyyuea.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rkfhplok.html


<!-- 参考信息 -->