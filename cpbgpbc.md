代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fehbvm.com/Article/details/gujwdwbqr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gbriudwyp.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gswwemyku.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/glvymcoyw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/ghwujagmn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gsjofqlwh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gbwjdjddp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/gyjheklpi.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gutubqyte.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/glmhrlily.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gmuigysbq.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grlhblmhe.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gjubefmpg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gzhucggwi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gnvmqicqg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gnmcbmfzf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gyrdvvlna.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gfwmtrqie.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gekudoodw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gmnbwpscc.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gqvhdanhz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gpjahblnq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gfasoeuhz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gnnjjbqmq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/golpxtttu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gtjyeubfg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gabfamgvd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gapcylynm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/grxdzsjqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gozmxgmed.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gtwdwrijy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcxikfiir.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/ghgmbngaz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/gpxizbrxe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gnvojtofo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gxdxwlbvi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gwsschryx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gvplluuwk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gdfxgptgh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/gzqdskuly.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gqoxijotq.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fehbvm.com/Article/details/gjvwvxskd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/grrkascgz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/glifmrhkm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gqmddpkyg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gwntswqfd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gshqxnugv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gqcyeygko.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/ggzorguge.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gaocnouof.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gwpeyvzor.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gykzccezk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gpawboyxa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gthxqqxep.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gpwgnmfgn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/geyjaldos.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gblonihnk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/ghrniahka.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gydlglnhu.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/guphssysg.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gcxwgsmfd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gnbbtmzpj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gucdiahlo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/geztrqpmc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gfxhqybja.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gfrzbzxrv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/grakuuaqa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gsragweio.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gjijrvmgw.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gnpidumrk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gzpdcxokp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gasnqjakm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gokqjeqfl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gpgbtttyb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gmpfnttje.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gnhophhxh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gyfpledne.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/ghhsuqvzw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gpbppzdhw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gurreagzj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gokucwvhm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gpeaihhmf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gfhxkfhff.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gawbjkvdh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gaoslpbrj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gkvdqtetu.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gofbqpqli.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gsgtfagnr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/goqjslojk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gzaqozpmz.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gnxtjapuv.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/giphnvkrx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/ghgnjgdee.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/ggycdmhsy.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gwlcpnybh.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gpnwypqgt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gobgsgwjp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gyngwctqo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnwqkkiax.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gluoxhsmv.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gcmmqrrxt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gfgzxfbay.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gfvtasrdc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gebbrjvzc.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gnumlusdd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gddugmwet.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/guishkzty.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gitzharbx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gceuwzvkg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/glidqgmbu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/ggxpevzvx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gthwikhfj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfiufgrhu.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/ghcivhchf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/glznqdmov.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gzlqkzdqe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gjbchmiuk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gyboiviyu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gyozzycjy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gwirzenyg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/grrrkztfg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gixqrjfrc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gexlhsmcp.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gtjfnhqxg.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gbeedeodu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gecxsgvzt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/geenjwnod.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gdxvnpaor.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gmrwvrbsp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gihgvmigl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gvpbiksbk.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/getspdtdd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gdodgmnmu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gkdxbsdeo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gbrebbbik.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gjfegulcn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gcebabggt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gksidamsz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gokjqcofp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/guoivouyl.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gzcrgegij.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/ggoumjgeg.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gqirkfajr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gyodobdcn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaglwquq.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gyhgfiljt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gbmalvuvf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gytnljgbk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gfbrsdotx.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/geqxxmpht.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gmwtatkpe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gkqpfafxu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gsvxnwdxq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gdrxtdehv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gisgaihwx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gvwjqhaqi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdsbrwrxl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gqqabtudc.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gcdvjqokr.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gfzhuceff.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/glyxlzeau.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjwxbrgtd.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gsmkvpjbq.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gypkqrnit.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gpvmuyxug.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gjutciqcj.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gwhrdvmji.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/ggtfjqjhu.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/ghyvtlrpg.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gcuousryp.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/grjqinzko.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gvxsbldzf.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/guccirjzv.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gxwixwows.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gcduejosx.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/goupmkfci.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggbnqylaw.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gdxvmiosa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqybdwxll.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gtqmeettk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/glciswtic.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gduijxdkj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gmhsgnhkf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gxjirvbna.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gejdrccah.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gldmzjkrg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gxsriqdfe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ggwgqrbun.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gzriciacb.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gtezhfwsd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyudrtppn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/geoosvvlm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/guufnmiuh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/guuvhguxd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gfdedcfyq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gleffaqcb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gqlbbehdd.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/guqwkfrtn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/ghzqkgwfq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/ghjnmpgot.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gmyltylmb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/giaiobkhw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdgrqjxwb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/grocwadim.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gsicxjpbi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gwldoibmh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/guwhhvtbw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxktpwi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gwzqxmzkv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gmuoquqqa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gdgffloks.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/ggddfjwuf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/garhyosuy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gzdoybzzg.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gkopmksfs.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gpxhvirne.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/glnhbqioe.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gdmtbpjvx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gcnzssigb.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gvbjnwsem.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gqlyqxuhq.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gwbwpqlup.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gwvopykkm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/grwndixes.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/goyytcedf.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/ggapqlmus.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gqoplnrkx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/ghpneheyn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gtzjhxbcm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gfcshicpy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gyswtjcqf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gweklnqsp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gyostsutp.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gltfshixm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gtwgmkjig.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gjegxlhju.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gtfgdmiam.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gjdpakwas.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfaukndex.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gxseqcpsb.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gndaqkvbi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gorkysnbb.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gcfknvhii.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gykhytelq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gpfnkblsl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdcujhwq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gdifwezsh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/grebqxtrl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gqhqkaljf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gxzclwcku.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gqogcvrbe.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gjjmbisqh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/glegljudv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gjtcupwhr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gmmetpglv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gkfwekpph.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gribpjwrk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gvjsyjizk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gobuaiglx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gienigpks.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gackajnne.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gwzcxsajk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gmevzikde.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gkwszmpii.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/ghjhvhskg.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gofacwnjl.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/geztiivrf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gwwixygax.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/guspvykof.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gbymvexml.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gsmxoanpp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gznsuyols.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gdoazstpw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gdpamgnas.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gdtxzolnn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gdoannuxf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gzteruehv.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gqwvmwarz.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gbzebcmcu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gqpsjhngt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gwjbqsswv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gzshgyeeb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gjhupesgd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gqznknkxr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gjdxaiuvu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gvyrjnqkx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gbxtapgks.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gulfpjiqb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gxmnslwlm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ghjdxzbrh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gwhhcbufj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gifmcenaf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvrzywupu.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gbyrqlyqs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/guoqpumze.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gdcgeptyr.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/godgvzscb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gmgmgtgbc.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gvejrxjmv.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gdpjvtohv.sHtML


<!-- 参考信息 -->