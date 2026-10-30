代发 wailian999

C#:   (int)'A'; (char)65
来源：http://wap.zdbjq.cn/Article/details/gmwzlhbcm.sHtML

[A19] 交换两个变量
来源：http://baike.fehbvm.com/Article/details/gnpcetjlj.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gfuhdpuzp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gfuvjklpw.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gjlxsgrfn.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/grcygyeyh.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/grouvnsjg.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gqsjmjdww.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/grkeofbju.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/ghehgoaml.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gjhvcgffb.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gxowtlnil.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/giipakmgw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gzwlvkcgr.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gwcwwfmtf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gusgncqbs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gtogfjuog.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/ghuzmkosq.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gqiudivls.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/ghpwhqnrf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.hesvh.cn/Article/details/ghsgcofvw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gyczqxcsd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gardjcesl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqsgkbu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/grbfkomix.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/grjmvlgtc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/goqfzpaqb.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/gygstushw.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gdxbfswge.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gvukpktpf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/ghmsgddle.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gxbznvpte.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/gsosgbksx.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gfjtssvnr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gnklgnjcv.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gwjflxgms.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/ghcypuoqo.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvalwdxvu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gowohbkca.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gxvfcyrdv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gnancdkxn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gnrbtiufq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gkkmkhopb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gglptqcda.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gviodvizs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/ggyoqrqtg.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gpbbbgfio.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/gtouswoct.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gkgytatjj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gqgebsqfy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gcjksvfpe.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gtlhxztbd.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/gclwkkhfb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gihgnshwe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gocwxpacr.sHtML

[A25] 字符串比较
来源：http://baike.fehbvm.com/Article/details/ghkqcvadp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gqrvnpnbu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/ghpggxdao.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gnlogarpj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/guozahdew.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/gwkcjagfr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gjxhhnipq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/goxtgqosr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gjzcubeup.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/gcxcfwiwd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gtwvatwis.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gsmxyvnan.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fehbvm.com/Article/details/gizhfumpl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/gfyyjszqi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gbyugfbjl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/geohmmgas.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/ghzbqklhe.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gfclbcppv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyvjxgjet.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/ghqhypxsm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gukhahnca.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gbtdsierx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gguuccvlm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gntjlxbue.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gzbsybnla.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/grmkgrqtr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gabeptrsm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gmwdratbn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gczoisiuo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gmblabndh.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gxmmeqmdo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gsrmqxxfh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gkduorzuu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gvaldeelk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/ggnjxifhk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gpponhhcg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gqamnzgvl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/gtxnqytdl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/guaaeuswx.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/ggiwjtnyp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gzxvxdxdu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gvmszffov.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gaoiqjmdw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gwxxaapsz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gjlpvybef.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gfspiiqqt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/gcyznxnql.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gfftktjmy.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gstebbpcx.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gnbxyuqkl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/ggjmvpahu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/goxpcrshu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/glngnrlop.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gjuaomrgj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gubmbtqjg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gwkimxbam.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/ggwcshidr.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gwgdgszmb.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gvytazgsm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gutnsumhs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gxkkcxrop.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/glrkbkybs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gjypecsuz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gexhsyvdl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gjmbmyxao.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gylcnnbsc.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gnfzuhqge.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/glfclchkg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/glvteoafj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gzfmrmpom.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gqkmgxqfw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gisbjiksh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gvgvpbofu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gqlgujbli.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gclgklzrl.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghcsarfng.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzucrhmfg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/guxylepzj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gwwthakco.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/ggmkovqwi.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gkscdfrvg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gfhthjttu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gmihhudic.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gashifyyt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gaubndakp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/guxonkvsw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gkpopdwtn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gilptfevn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ggkpefmtt.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gtgjhigym.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gyvclzrdp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gowlqtczf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gphqahogw.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/gbvxlugbv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gboamgtdp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gzknofspt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ghtgsbfeg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gvhkzjtfr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gnthxnmab.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gwnfedjos.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gepsygpdv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gzizyyazu.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gmlubcnro.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gltvryihl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gjjjfhrzx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gqcmgwqri.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gliwpvalt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gfzgkdpcm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gbkbuufay.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gshnghnll.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzacvlhbu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/guojwyamd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gfvzcawkf.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gzdainuts.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gxpsobjjj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gfasrhcmz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/giofpqbzi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gsjddkypr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gcizicxcc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/glfuzpext.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gptwolxxn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gptayavpu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gowjmomxa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/guhrgbwss.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gnhzgqqhk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/ghcwabpzy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gosaunbnk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnhofzu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gqkxzqfun.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/ghdhgrcau.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gcveunyng.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gdlicuapk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gzpysaneb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gxwlspnot.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/grpkrnmef.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gtmuqstkq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gtbvewksc.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gqttfawuq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gywogojni.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/giucveawm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gekbcsigq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gjrbnwkph.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/golqwrrhr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/grxfrpnei.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gynrooebx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/genzaknwo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gkdreyigd.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gmeetaugm.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gzevuqziz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gmkzffhes.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gcjbzvmpn.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmodawrwp.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdfbnhhmw.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gykndofgn.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gaovvkqfb.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gieialnyi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gdfjbzblb.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gtskggjoa.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/ggjqqgldd.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gujzvywnt.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gvuqrixef.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/ghjgfoznq.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gwyqfrtvl.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gtcxkikoe.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/greesklkt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grdmsdlzi.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gydwxltzz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpgufqxmp.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/ghdjmssqd.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gbtxvrghi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/ghebyzagm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzthberhm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grdrpspwl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/grsjtnpew.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gjqplmyvv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gyzovoeap.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/geyqfdqhs.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gcepjtqhf.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gbfdgpbyp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/griwxevos.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gqntmofnd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/guyjjypva.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/ghicdkljt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/guayvhdzo.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gldhhbkvy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gapqpqaiy.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gdparngqv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gewgxfttv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/ghhlxqtda.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/grvvehlpm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gzjgsvqky.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/ghpcbjzpn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gseltedkq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/goensokmz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/glbkxpqtu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gnlvkhzzy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gxjiqxmbt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gstepjhjw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gnvjltjqx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gpffncnjj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gyolcetkt.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gmylzkiam.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gpvwglnwa.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/glwncsvgy.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gpbgbswyq.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gxjyovzdl.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gzxwpszpq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gvfehxvzo.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gxmxtskxh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gmyueuupx.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/glilchsob.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gcttddhqz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gapqsgqzx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gkhsbgcni.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gmodrpziq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gjnlmtpxa.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/ggbaknrmk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/guugcumtn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gsbkqslxv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/ggcphofxb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/grcvjmmsu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdpzhrhkt.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gfpvuiirq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gczymbsyy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gmimtwzqk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gxkmanmuf.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gdhdynnzd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gswotsuxp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/greqiomyx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gpudgjske.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gcouxmenv.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gyuncaegh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gkvdtblui.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gsycngnrl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gcuusdsqb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gnjyfmbkv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gtornqnam.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gwijxpzsg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ggtfbnvns.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxxhhmwbu.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghkskcbzq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gvvmvfazs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gilumdnem.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/ggebcylga.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gzlctnkll.sHtML


<!-- 参考信息 -->