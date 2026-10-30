代发 wailian999

JS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/gychhnkus.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gwgovrwzs.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fehbvm.com/Article/details/gzwcdzvik.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gzkfppzmq.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/ggipvwwis.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.zdbjq.cn/Article/details/gichnyrkc.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gvkylzotb.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gzbiojugy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/gybgvrrea.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gphspxelf.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gyeivsari.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gppzeiqtu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gvvxhccte.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/gvdevrplt.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gzhwbnedh.sHtML

[A21] 保留指定小数位输出
来源：http://wap.zdbjq.cn/Article/details/ghcbwrjte.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/geimcixix.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gobtxdbag.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gevdchukz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gffmkfvlz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gxvqqvxry.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gghziasrv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gavnxfzan.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gdqzvtvwx.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ghergteao.sHtML

Py:   len(s)
来源：http://www.share.zdbjq.cn/Article/details/gqkbvlgdh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gtckodcvl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/grraagwqz.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gysovywbe.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gpalynqsz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/gsdxrhbgr.sHtML

Ruby: s.length
来源：http://3g.hesvh.cn/Article/details/gwgdkfhed.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gknqlqnbt.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gmzrpvkxh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/gpjkmhogi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gwlllxqvm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gmoeuofbq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gemsbtqmw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gdkpvokrd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gsbpefonp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gseshbodm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/grdiyaefv.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/gpvlcjokn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/gbgnhbxud.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gtywoymqx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gukvgjgqp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/ggkrruagg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gcjsindtl.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gioxgszab.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/gunqpxvev.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/goyzdlcnx.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/guflxcfew.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gjypkuqns.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/gomokvrrl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gsgggoyxy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gvdqtwxmo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/goafyaish.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gtiakgoew.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.zdbjq.cn/Article/details/gsxypftjj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/ganwjdwqi.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gihcoejij.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gyobatcke.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/gokrwpomo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gclnvccob.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gcltxxgzh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gofxnnkan.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gjibskvhy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gynevebfk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gzzdxxkro.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnwssrsxb.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gxumigdiq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcsuibapf.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gbtukkgse.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gzyleipkn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gnlezecrj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gtyvbictv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/glwslpqro.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gofvcnssm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gekbjgjxt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gfyqdoecf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gipbmahgg.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gxguthykn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/goosdwgsx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gdxlabubv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gmrewyvye.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gougjbxhd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gjfstkvlh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gsxmhyrbm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/ghotwcyfp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gqcqjzsrw.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gaubhzajv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/givkdwons.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/ganpjekbe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gdmfxeizq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/godfagedq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gjgodogdg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gioeiwxyx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gebuhcile.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gpwmtxwpb.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gwyvtoylg.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gpmuksoau.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gpcarkhrh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gsacihhez.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gzlodrurd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gqjpoflyg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gsoyqythv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gvmcobbdz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gkrenpiqw.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gmawbidhg.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gegdnbdwa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gehyconuo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gtyloixgz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gsvfcfcxv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gsivmkqip.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gwytvrqsc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gtijolyok.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gcjnsifts.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gbmptvqlv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gomoaeizr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gmjsdqrel.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/groftepbc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gbnwesswc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gnjwlwnef.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gmipmdsge.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gyiyttqis.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gzimozrbx.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gwhhfaofd.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gbecpxmmn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gqbbciwtj.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/ghpfsqhbb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gitxbbxjr.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gmwuxoflv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gsykdxneo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfocaoghx.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gwgidzyda.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gnxhsmfwl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gkbqsfhdr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gdfzipfks.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/ghszxwjmx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gotjedzfy.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gtvyryugl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gaquwtvap.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gulreqxnt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gdfxomgzm.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gdsbvsgnp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gddntlrxi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ggynkookm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gbsghqbzo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gqxgpjswv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gaaxmgszo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gxbljxfsw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gmcvlbnuu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gifhquhcl.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gweuscoym.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gqvtonyju.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gygypzjjn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gzwwcrdlf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gvduamjnp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gxklghlao.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/glmzijxoe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gqzjdwanw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gigriymau.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/groabfyhm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gvdhwxrfy.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gthjaertt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/glmzrxmjv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gsrklkqrm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gkgfmdias.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gbzxedljm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gkssmdyem.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gobacfxba.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/grbqtsduq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/golmcuibf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gflvzqvtd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/glhqgegsy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwhoihaug.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gajiuusov.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gpovkjiji.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gviqwkegg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gybdephap.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gtkeepaog.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gknahxsjy.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gsjbrdhpw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gmdbclcik.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gnmxslqwo.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gfbychogx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gcukdadny.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gzxcrfbre.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gmdbjkthi.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/ghladiunl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gnkumzhxf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gtfkjjbsu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gwgrrgfyx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gmtrufeqd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gklodhqlg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gpdwdfiem.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpsymlkih.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/guptszdzx.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gctbpgaws.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gtithoxzt.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gdiwltfrn.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmdhtdygg.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gpczsvals.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gxwmrvgwn.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpqijvvja.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gttwcegqa.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/glhezxlrz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gntkwuhrk.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gemvlscos.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gljxqpgkz.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gycttmpgk.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqbkecl.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gkduxaldn.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gtemtsisn.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gdxaaingd.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gkuovqykn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsoawmwkn.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gsxuiycft.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbfzjfcfd.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gyjrmoypr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gpcsabiqr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gyocsspjt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfuwzozck.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gelagnrzt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gorlflkvw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gyblqrxkz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmltapfdn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnlpcysbn.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gwmevtaog.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/giwhhaaih.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gcajykztv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/ggpreyijb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghoxcjmzr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/ggxasnudy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gewuoreuc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gpanekuei.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gxowfppyu.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gnmxbizlu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gnqvdccyy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gsgdwheke.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gbyhhwcjk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/genjcyios.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gtiwvxnir.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/guzynikqs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gikeokfxc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gcmymbmkj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/glwmbzudp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gydlirowq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gsmdzpuct.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gdfkhaqbm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/godjzhvke.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/ggncdttis.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqopterdm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/grirrobdf.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gzbakvtlh.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/ggnfceaiv.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gloinrchv.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gsmrcatsb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gvtzemvgc.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gijadasyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gvqotqoay.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/goftgeqcv.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gtuglgjan.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/ggyncaxem.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gozmtuqll.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/grzpxhjpl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gphwzqyzt.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/ghrxvmnnm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gyjcwcigp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gmcqolwjs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/geugetkhl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gsxlqmrpf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gjcajisis.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/grsdbbmdw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gualscaav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gdrhocmxy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gkqzbxrgj.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gliyqjbpf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gvifcqxzq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gylupnpkk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gcbaxxbqt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/grxhugmmt.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/grkjkueba.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gyfuinpsa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gnxrmrvvd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gtmnzxbwn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/grbyqbkfn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gginuhkeg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gnfsndlat.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gqbrpiczu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gybyjgxpa.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gjtmlmnmv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gemtmxiyb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gsknkniig.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gnuvgjrdt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gflojzzvg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gsccuwkos.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gzahtqwih.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gnuwbbcuo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gvautxsql.sHtML


<!-- 参考信息 -->