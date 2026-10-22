代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qerzkwcv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2roocongi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2qqhdilig.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bdbzvica.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjkjmxoh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pmmrhkdj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tnraefje.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2llwetywb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlqgiuvw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2duccaqrg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mcnqveoj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dgncewbe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zlhfzzgx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2oazripzl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qplzmteo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhvgpcd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2taljwcrc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbkpneqe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2hyfdflwb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqudjdp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2fmnfjekf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qhglzipb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2motcuhwv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kyrsuqvc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2zviickgm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gjgeuqfx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2akbhstyb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vuubzcem.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2oopirfxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mecpycyh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xcbaskzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyedulua.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hzfntiok.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2czoqztxx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hzqdxbgn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hlfzyewg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wvhwadql.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ifyrajnh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cuesvjas.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vauyjswb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yxyszokt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kbxwijii.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qjytjbuz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2edtwiirj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ezqdzfhn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dimykapn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yjvaneig.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2elyoumcr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mndxifhc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2axcijzwq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2aexkclvp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2heokbkdo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nwuoezwk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iypsxhzl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hifwzxir.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2snbhtlda.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kmkldszo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2zdczdgcp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2twrlplse.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2obcollsg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2brtryyse.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ngwtcyzu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2svielyrs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xgyokysc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fzmgwjft.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2srolewir.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kcvleufq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pcgrgipf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ecqspkwr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2limkmwjr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlntcqxz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2btycldgc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2smqdmdre.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2wiuwufvb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pdmhhgpi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dzsidkxi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2scceyvaj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2osfaekeg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2icqdwbtu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qegcvnhj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2oggecuqj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jynshktj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2npvehbyl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rcxnfkav.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2sylemysm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2oliejnji.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fasnphyz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqynqwtb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2olpasozm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tzqtmenq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kabvzeyc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bnhyukbk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ddatussz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jxknzcdi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgwdnqzt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ybwtgcsm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ajcygwkm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2stkkqerg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aywkyzqm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nurbpdgv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xzanwdpt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cctcnget.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dufuggva.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2elupymnk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zfyezezy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yvherdzo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cebzsjgd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydlgrnfv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqrstqfx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2exawamyc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kzmxwdiu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2lquctmhm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2btiinmve.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ybnvqbxs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fltozzpw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uughazzl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sgqfmgsr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gvhnyyog.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdimfwhg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vrudlnnb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gtbdtxvg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jayhnrks.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2isyyzlbc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rouxcqzh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ubgvliby.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pxssdhgl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hdzankoz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mzymdxpn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2phxqudsg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2brxzmfxq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2djwsgtsp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2biriwkll.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2slmgaxmu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ituwfiyc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2azohzvvu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bezuppyg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jakmwawo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ownnscjm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dmdxglyq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hxhfkxwg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lmekbrxj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2edyuovud.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfembwmi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hqdnexem.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nslpwzcd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vyecmaay.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2enmuldbo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2gxchmwne.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ysudehgo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vttdbzxh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dsuhfvhm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xbvmyvge.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eztmlbvu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wwdpunug.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ybvntdzb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qljrtbog.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgscusrx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2neauxyqt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nkjqzgez.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tpbjwwvy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qvjmeeld.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kpmsszae.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qmtrqask.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tptxffij.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hvxdbhob.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ythxaufv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bvsomocn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jdjfffvk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2snvdqtao.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mrcsbzyq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ikwopqfo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hrjpvzkj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2chjwcetg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ukfdkhzx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fbcgldpo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mnnjlols.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjgdokqk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zhmsgktz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xybpohsr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nycocuim.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2svmnifrq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gghsqqce.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sznmzytn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sonxfqfh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwarplim.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dwdtvvmw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fnljhzmc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zzdcwnau.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ivdovljz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mrrworyt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2binlufqi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aryzltxh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbuynqhp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tyfspnlc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbpdpbqw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2aseahjpm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nnrvvlwf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oxvqwlhk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dprhxzul.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bmbsgiav.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sebxcnrp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjuevohr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gkymfznr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hsrrqpum.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2umecfcia.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ahwtvxyw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2dqwohxrz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2izcwsijn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rmqygdhu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmabqbmg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2crroqqsd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hdhxpbcs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ywfnzgmo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nplufhdh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohurathr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qgfbbroz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dzkjlvvl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2itkznbsi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2klksidcl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2snyiboee.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jbvnzevq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eyeawolf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2biwwwdep.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2surnijwi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wieememk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wycuvmlv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gouecaks.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zxupoahv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ppeuphmv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xenhjbnj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vlnctvoc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zmyqhtia.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wqjclicu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2eaooldmg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmxoxus.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gtrbluck.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2htbgwqkg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2beqtieqz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sdutxely.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fpbtcecv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qiygkdok.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jqjmtwrv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2khtytbsy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sgvhfcrw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtrrokf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2userxjxl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rkapkpgj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jonfjxtk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhsjiqzd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2byaagabx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vikrekvx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2pwwjakze.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mynnsyuk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnlarztz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2obbrvvyu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wlvuarjw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tbdnxvxs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mvftgywt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2odepdxxb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hauvzwjz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ujdlirbn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vtpglwws.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2eqsbjkcp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ammbqenb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jlqztwfd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xoplumqe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sfdfgshz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nmemjmhq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kugcvcjq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ufybnyhd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cladynog.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nfuypkfx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jkhnigrd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rbrlalma.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rzrevkbc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wkbfviwh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zzbvtvlf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cthlzwlx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qcjyyhqs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cayqufvv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ohzostfp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sryjpcuk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lgqjdgew.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gvvluhlf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xaitxggx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bodmolig.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kvarwdbt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uciwypst.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jufnazlr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzljpujy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zgorjkxz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2blhkhwim.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mubvxokw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wrktfzez.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2umnfaolx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jvcvzwxa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgbsmktu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mggrcidc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hkggyfod.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2idwtlatw.html


<!-- 参考信息 -->