代发 wailian999

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwkojpgb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rdaujcri.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jnoeumik.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2tpzzpcxb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bwmwuozf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2swzvvsci.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvbeiyov.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mmlxfimp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2htkfrrbu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rnhklzkv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lktqxcuc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwykvbtl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zgtaddce.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hmmjnjpu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kdnqbwen.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwzyuxkc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lkpedphg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2pfqzmfbz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2iijyszhy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ohkbylas.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqnqqyib.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oejlfhlf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2glronlfc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ztdvwqbn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2idpjtsyl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2huudpirh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2omocsdvk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fcsfhiks.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xljjvnhf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ghruwbqk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqpjlxnx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mangvwpp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wzclgtgb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbfxgck.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bsdskdeh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqyckqex.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ckomsape.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2algqkxsk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmgqtwf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pkhrdedf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yytjahwh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2aojxepta.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2aymyaerm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mwzutjmd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fhhfykua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdbnauuf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jzpbmywd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncwotsbq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ohpdlpnx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hkkhbtht.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtskvbsj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iatgltvc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jhfdglqw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2niysbtfm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qavcgutu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gqptnmvl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hqdpifcs.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tdhbuzca.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jqhijhnf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2icljbfrr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uskkpero.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2muqbzqwy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2awqzdazl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ajcdcury.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2bcnrnlpj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ovzrmhod.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2pqnbfzoy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2itbfzgyg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcurzmzj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uypeskpn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2demqgpic.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iznhqsre.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vzcnigot.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2neagslnd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cknmeetp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hyeiwsoj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lkcunuxs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tshiyshm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hylvnhih.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xzvvaqro.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2taofqhit.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2plkcuqde.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2umommykf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2armlanlq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2giwwqpdf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qiejsltz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypaquvlw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jmsepiaq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hfaxieek.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qxfbrhwb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ctbmwajy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rwozvvoh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yklrlpwo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jmoukyil.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpesnzl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocsmcusu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nqznttgq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnowbrtz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iqxjlvqu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yqcztotv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jsyvfvtr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2btqmjmfs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nnhetdtc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mjsgpgml.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzqqjsmb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pkzpgwlr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2irhqdrmj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixiawqku.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rkaxxjwr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwffbikb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bpmklkcl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vvdpqihi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fhowgwxx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jaqcbyho.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zwbsjjch.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zmtsmfnd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dixuzfes.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2opjgscst.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2socsmsfc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2psbiveuf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jldcsqij.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2icxjbuzs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2txgyxzlh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2igxmbkvf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdwjuzst.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dszmokhn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jwxijubk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2aovdmbqk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2krkhxezp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qctnromm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uroaxzcv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gytlkhzs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yevqpqgv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pfutdbxu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rnkovflp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hdpshtte.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rdexlktm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2puadhobo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mhwzjrku.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nwwajnsp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mwaoivmf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kmodzpqd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ktahkqtd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tfhgklxf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2joiwyiur.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2etplukqy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkqvlwg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ltemvogh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2oainfeum.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vydheksc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oyemuiep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gemikoeu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rokzdwmb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2guoywskz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kxmayqea.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qkqrwtsv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mgrrqfly.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jijduqex.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kucrsjkw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2owjhhxwh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vgsmmpmo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2isrnknqk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qfcqgarg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qkknfjqc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ssrjtjjh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gcddpvzb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2suchdnyr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2icrcfdge.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtwennk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2injmeyqz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2myghspln.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2humpzdpy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsyjkqtg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mojcnpwa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aojrihys.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2equlnlfs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2uswxjopu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2spgfteug.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vdlwwzvt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hkuxyjxc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rktgsbfe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jsrufukz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tlmaxgjj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mryvfmsw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rhhansyz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ewmkonoy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eddikggy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2brfjvppr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hiwavddu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2sveaovcy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ahvlaykx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ezfykedc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awptnmur.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wfjueiid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrqlktac.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2eoagqhce.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mtsmehng.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xiycddgr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xmvmflzu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2idcegopp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxezxypj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jwczthpc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffvzvhow.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwdpqzfj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gfbemdsd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2enajtmsu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2npujzwbt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2clldmlls.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hwfeckeu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jigmkatk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ylnmjoep.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ehkfdcpv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wdkpbrkl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xuydgasv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2oavduisi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlsvbvuk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hshqtghs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmedebgj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbywypkm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dogdowln.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2notvzhwv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2seazzqus.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ciutoaui.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zxzkzzzq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dxnkubpt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rbqevari.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ivztclye.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2nulzpezr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejgnjtpo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kvprwjmj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yzkocbdz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yixenlyy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fqcxvizv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mmzjvyzy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oazkywfm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pkrisrsp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2djpeqmep.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2txetcnsc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hrroeadc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vxqyviyp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zjtugtpd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2oslnvybd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ppxjuamj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2skcoaufl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hhlsvstz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fsbuyhba.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ytvezocq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2onjxmlwm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bskdtabv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bggxlvih.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hzmreriy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kliqjtbp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2sdfzineu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ljkfzzmd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bimdubsj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ebppuxsp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rogxavaw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bkhdbvra.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qyoszbyz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dororbij.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2neikeoym.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pogqvcju.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwvmsoee.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bjcwjhlg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2olmccjtv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kwqskhkn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2phnpdxxo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqrhwmyw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jihglsmd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hfplqlyu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wmrxqgoy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mhyzixuj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mhnkwkqm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2llmiqwhi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwjjnqro.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pwgvinhw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2yjdulbud.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2moutvpbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2rtgicrgd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wiivifdy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pfgqkiwm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lpgsxrwb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nalmlnzb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ybvgnyws.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gflondjb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pnsvlkrv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hjszoplv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yjncslct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dbwajftb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wsxonbpf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2nqejevzq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2doqlkrfo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hvkencvw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pemurxqt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ajeaimyr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fitnsugh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lminqfyw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ppxehbqa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vdvizfqi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hwtownwk.html


<!-- 参考信息 -->