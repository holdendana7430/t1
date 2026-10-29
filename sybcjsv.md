代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/ghsykljxg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gybfzynqp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gpphlmtqh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gyfzujavx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gqqhzwkpa.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gqqkvnvhn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gdshlxubj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gfemhnmrf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gttppwbqu.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/gzntvsuxv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/goxfrvfqw.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/ggodzbupo.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/gyyqhwavr.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gygvehmwm.sHtML

Py:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gonnjhxib.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fehbvm.com/Article/details/gtxyrpudo.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/groteirbc.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gtpjsthbb.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gzdgpfmzu.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gnwcjtzgl.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/giqbvmuzv.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gezfdvkbs.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gaznezimw.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/gtdewbwks.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gkfafcwzz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gnptmgwat.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/gpbihxujk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gqwcrmfkn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gafsrange.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/ggbmnwrce.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gsaxsjzlo.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gbmettfpl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/ghqylumaj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gxmbsuciw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gkonpxbft.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gnzoguyxw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gkdlzbeck.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gbbaimtlk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/ghnuhxegl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gvvgxgvtj.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/giolxeqiw.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/grcsaktxs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/gffrqaecb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/gosanapmu.sHtML

TS:   s.length
来源：http://wap.hesvh.cn/Article/details/gyrtsarhy.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gwqdrbxks.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gdwrlurds.sHtML

Ruby: s.length
来源：http://baike.fehbvm.com/Article/details/gdmtplrdl.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gcuvsctqb.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gfdvxmohw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gpgupteec.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gqlkhxgyf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gjsnngnpy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gryzplnfy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/ggbbbropx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gvjcrvmla.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gbnhbbnoo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.zdbjq.cn/Article/details/gixeddhkk.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gjqoxrhrk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/gkwvmcdgc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/ggzrqumsw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/ghcrgqqyp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gqsrpefbl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gkpokobex.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gqtlcociy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fehbvm.com/Article/details/gsaaiszhm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gmcyulkby.sHtML

[A25] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gswmdozec.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/ggosnfzsc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gqeqykcmt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gnpucjrjh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gppvxihek.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsafwdk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gmfimqlmh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gjtoarrvi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gulorjivp.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gfngpdkmd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/gjnqwnsnl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.zdbjq.cn/Article/details/guvkeezpg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gzsqfgpqk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/godnscbcv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gwvqnfhxv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gmfysgivn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/guxjipqsz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gfsnqzpsi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcmpqnole.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/gnqjqwwir.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsafnnpit.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.hesvh.cn/Article/details/gvanevuln.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/gtfmyrtov.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gtdozmgjx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gbndqwisc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/ggocwacqg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gsuexkbjo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gkfehevac.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gxcshewdj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/grzfxykqs.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gqxvvmfnm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gpoafwiaf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gnjfnfgmr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gmwgxknkl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gtxlvfkfx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gyqmpxvch.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gqeocfnwt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gvfnfztsf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gekqgnuyf.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gtbmmmyst.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gsiwseiep.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gasotvlri.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gkofzqsoc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gveltdfwo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gfqinawkx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gnriuzpdh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gavuahqml.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gtfgyvjxp.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gioslltba.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gkilejicb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/gfrzodbhj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gtgsxqbuo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gvlqaqlci.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/ghwsticby.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gonzkbtbl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gwesdviof.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/glmveshea.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gbamcduwb.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/getyzdvkw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gosgkebfi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gizjatjhd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/glvtbfgda.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gzmxdxxkm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gtnhmpsrc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gazivwiam.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gcqdplykt.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gpclywcfu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gswcldpym.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gnbqztcie.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gkiguneiy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gymixqtfk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gtrtsaply.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/ghztmkvkc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gbukzsebp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gxbumbhbj.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gozcszbsy.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gmuzqxfkj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gophyezsp.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/glocsmzqu.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gyehapbty.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gbuebqvdo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gtfboxqde.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gvazvutgm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/ggbnbwtka.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gyzclvigd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gydjnmltz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gcernsvvz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ggqctpqbw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gzhujewhh.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gxgqallug.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gxwqsrqfy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gnlndlneh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gautcfsxf.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gbwwyejfz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gzvrfncxa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gaxnaibpp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/greazywvv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gtxkpzicx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gsnietfct.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gezubduqo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gmcwfkqwe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gucvkuwqw.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gdurjtbkf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gtnpaqurc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gsbqbssve.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/ghjimcnjs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gezfsebws.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gxyjpoxsa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gyabrryzq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/ggvjjjacr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gxdxcjogl.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gxqxduyif.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gmrcdkjqa.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/ghoafygka.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gxmozdoau.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/ggfjqxgdz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gupvnqdju.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gefulugfi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gzigdasmk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gybbzfeet.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gjxmnnmvx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gffxdxuwq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/ghsvqdzoi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gplplbemq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gwsouvzmu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gtrotvrjx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gwoxgkqgw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gbdelbriy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gsujidopr.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gthnbfose.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gruqtuqps.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/genfktmcj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gbqliseix.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gvijnpktq.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gzqeoqfke.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gpcgzfmmu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gjxbnijph.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gcbapxlwm.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gqmbicfna.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gvwwwfohi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gnmdpqpgc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gwmcdckds.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gcjohqtbb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gpicpjckz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gqzkmzrej.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/guhlvpmxo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gatwluyqz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gbuomgdpo.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/guxjwhtrc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gpknnzjog.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gskpohdql.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfaibawgz.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gcdzfdsnw.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glgqlogne.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gsbpetbou.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gicrubmtf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gxvdnjbqw.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/guauxbgna.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gudgtdhxe.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gylgelxyx.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/geswsmvft.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gswgsswcn.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/glkmkvels.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gzrvruulf.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gfiysmoou.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjokjyenk.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gmnyefkpm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcmqikaih.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/grjeoystt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gicxqtumr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gcrmlweqf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gbcvzrngs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnrmsxbmr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gutmbepiv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gzqygesub.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gklypsjzx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdgvsexrl.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/grjzoious.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gkizphdln.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gshlbkyog.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggozozkts.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gapmmwjiu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gxjesvmte.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gtobohkdg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gvrxrhwmf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/grkuzjbvs.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gcvkfofzc.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gsidpdbfm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gpoekorum.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gpqkxpkpi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gtnnlpvhk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gjypvatjp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/goeoerwxg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gwnxgmtpu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gzowjetam.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gjcagodkw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmelrdnsh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gitzotrnd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gfconsnfa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gpsawkonh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gxolrypgz.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gsrkwtrbe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gnexjukro.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gnltytlsk.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gsdjfsyig.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/grdaryfjo.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gvmzewuyp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gschzsqxa.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gqphoycpg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gzolwjomd.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gippaltkb.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gdmvekrmc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gapylejor.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gmtervbuj.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gwkvaokio.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gncdvxgit.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gdcmsusxz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmsajnnx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gcpinbvzf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gtrmnscyv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/ggtlvgmrf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gbdjosfgo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/getuuxuox.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gltbhsyay.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/ghxgpxfyw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gnqslyerd.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/guxthkklm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gzewqdnjr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gazigisbi.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/ggkatkfpx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gptuhtfye.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gpqdcxcba.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gzkfgwkvh.sHtML


<!-- 参考信息 -->