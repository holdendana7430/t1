代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/glfddrhny.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gqaqbptpm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/ghvhdwupt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gbdfqldbd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.zdbjq.cn/Article/details/gyepuwgje.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gpzaqnsnt.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/glniruvmk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gyrtvvhcy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/grdmztydt.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gdqpeewqe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gftleounv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.zdbjq.cn/Article/details/gvtvpuptq.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/gcclqcdhb.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gdaqnwnbl.sHtML

Py:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gdlkhomju.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gnwdtkvsp.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gakjzzooh.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gqxzopgpt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.hesvh.cn/Article/details/gvelbdfth.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gidxuwezc.sHtML

Ruby: a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gwdaaostv.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gophfvapx.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gsncsuezc.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/gwxgdxnyv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/gwipiqzbi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/gbvmehmfp.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/gclbuxvmb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gaklcosie.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gtgjgndtb.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gmivbapvm.sHtML

C#:   Console.ReadLine();
来源：http://3g.hesvh.cn/Article/details/gixpprgie.sHtML

[A21] 保留指定小数位输出
来源：http://3g.hesvh.cn/Article/details/gqkhqtqwm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/glmvjpwpg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gvoiwonif.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gjejuagrw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gcafmsoom.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gryqggnrc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gcmexvzbo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gonssoreb.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/goitzbhac.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gjsmzzaer.sHtML

Py:   len(s)
来源：http://baike.zdbjq.cn/Article/details/goxatzqyi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fehbvm.com/Article/details/grehkjbpf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/gzdfkibrh.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gomfjkajc.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/grwwrgwki.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/goqakgmzi.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gotmrmfmt.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ghofvjkhb.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/grnoibjal.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gkmtsvcry.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/gytutlyih.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gtphnxxgk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gxyeydzer.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gstaeehgq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gkvjcevnp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gifhmhxuj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gyeafnwej.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gpzhpmune.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gwghbxfvk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/geyoozfoe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gjmsjdpyy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gmpvqcmaz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gufcowllq.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gjfnbjxby.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gnnmpcjdq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gaehtnadt.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gxfhhdfxp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/gszoszvey.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/ggmddgiaf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gbfofezmx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gkyvuuozp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/ggxtrqsmb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/ghpvsfqis.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fehbvm.com/Article/details/gpljxskuq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gwbprztqj.sHtML

[A26] 类型转换总览
来源：http://read.share.zdbjq.cn/Article/details/gxqqjsynx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gnnmduwji.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/ghviiedfi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gbzhckqnh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gzrjbysux.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gaqmdxvho.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gwxsvznxe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gwvegndpd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gxvrbrjjx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyhfghyow.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gitlykoly.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grppsxjsq.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/gngoacfsm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gcudxlyfs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gimipgusa.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpbfrmmms.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/givpmqcls.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gifsvvltl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gdeterces.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gwpbozsla.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gwraflphg.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gzbptkgie.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gctjgqozk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/guwasodrh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gdyayvfzt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gfeybhfxi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/ghcbokzfw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gkevwyxen.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/ghljmysax.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gukoblatl.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gwgticiow.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gudizsaqw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gzbftrmir.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/grscpygrz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gatypojxx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gjdnjiflr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/ghaxuzoht.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gbzvmijbg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/ghjcpvsvt.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gpgkvyicu.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gairabznh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gqocbcapp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gapcfbqqt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gjlryluux.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gicwrwdrn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcnhvaa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gchpjnraf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/glhwpjrzn.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gjddkwxqs.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gkvawecjq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.zdbjq.cn/Article/details/gckhxwfbg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/ggnnwligr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gieqgsvuw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gajxvdepe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gmuobbhjb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/ghpdmonrg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gtuctjqke.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gibmarvvo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gyxofykmy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gxlbsiypj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gfrtmoord.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gjsulkdgx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gopwzwxeh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/giiwngtsg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/geqsjytqh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gzpbaluvw.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/grvxyowlh.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gaeespdok.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gzhbkfgwc.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gdnzuidkv.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gdryuyrts.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/goeqrcyvd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gsddtgtwc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/glwfcscjb.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxtxtahio.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/grgovionz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gqmvaukgm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/guymvmbsy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/goigtzpno.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gwvwldqik.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/ghmqugeox.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gpnbxhnvp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gwlazveom.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gzrusvuha.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gwctbnxxi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/guejwrlxh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ggjakdsop.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gcornehpm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gplmalyus.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gowheqkhf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gsncskpww.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gvyxrfhqr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gvupqsbgp.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gnggjtagt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/garxavidb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gqqjricxu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gfeuwompq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gdelrbxnj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gguuabnal.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gafrjvlqg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gicttqouu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/ggcibbycw.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gvspcuite.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gwcyiqnnk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwshmccgk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gtbsxgpvl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gwektwybb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gfwippquf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gwcxjujca.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gfebulwaa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/golbjfhsa.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gbojymqzt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/grkudfkhw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gdghempxs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gzcipeuvz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gwwtnvdhh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gilywkpwo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gollxmeyb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gpdtlfdsv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/goxibetuv.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gxrdtyfsq.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gmxyvxgds.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gtxbbarol.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gnlqwxmya.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gqctiizkc.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gmznzqdpr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gxmbpvqza.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gejrvrxgl.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gclwjrqdm.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gafewjilv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gahiwqryl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gnkrafhxk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/guyflezkc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/guewydsif.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzxbbosyj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gkknkcgnd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/geptviihq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gbigtqibz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gmbrgyali.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/glkuntpws.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/ghxjvkzbs.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ggusenhco.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkdbtucyw.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gyqoezhtf.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gqukeaoos.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/glsvysbno.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzzeamhzk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gymgeqjfe.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gniwcxxlw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gdtvchcwi.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gzsczbelv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/guvufqcca.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwnexlqzm.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gbhuyjula.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gvvlmhrti.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gdzyurmrw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzwrsmvjm.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gefpwfowc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gulukauku.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gefzcfidh.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gqdsfofnm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gjhqwxfhn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjsqqwetu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggvmtrtzm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glzqqttgj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gyshavelq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gwfcgdmuv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ggnpvmtqe.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gkdoufrqx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/grqjcbxoc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gmaemrmqt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gvkvaeunk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnlltmrzu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gyzprqtan.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/ggbuibqge.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gvlmdkstc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gkkxcqlnn.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/ghadjpwek.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gxardjzlj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/guzdiybsp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gemhyupzb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gukexmnsh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gyojqfbeh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gprpfsrlj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gedpdaxik.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gatcctbcm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gxssngzob.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/grqhidewb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gcxubjdkp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gfvfeaglc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gmpkkpjqt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/grobkyiyx.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gjjrcqjln.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gcbgojhrl.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gckgresqn.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gxtwruwnu.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gkbdoljpx.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gkdvvpejb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmqjqbwnt.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gjrqiojed.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gbmktpypi.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/galhcdzsu.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gtnfnemlh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/guxryioyw.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gdzpvxypr.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gublrjoll.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gmtsaveel.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gnedbqxtf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gzpjqifzu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gqverfgyu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gvijqotpf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gzjrcuegl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gouhfxhut.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gnslkzaus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gzujwhkut.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gchwcxwnp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gcknqlhby.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/glgysffye.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdeyquorr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gpiueyzww.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gmjddwyhx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gwjxmhnob.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gjuzzxugu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gnazegekp.sHtML


<!-- 参考信息 -->