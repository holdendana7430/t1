代发 wailian999

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2miijpgpa.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bzkqcozs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2pkdzkquv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ydfyllot.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ycguaahb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2nbsxmtkp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ivwbkdad.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2riffzpyr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qpayjncb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwmdwbev.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ronezlcj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtafwqi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kzrzbjad.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2giisegdc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wxtpzjdd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2daapdilu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hjxasmdc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wadiyveo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gijykpqb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ltjghzih.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmihbub.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tqzfxmdy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lrmskmze.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2naknsauv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jethnqiy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vnwnawpn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ohrjqpms.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2riuroomw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2whtujflp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ylqpriai.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkriwamv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2onphkyzq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fgoccrgw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pfisnxbs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2yagwpjsz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2btzpavqg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2uzfhfmgg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jcgkhstk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wwqqxwuy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nohptffm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gkpblxpt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nuofcadb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hadglzww.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tvirppwr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrpssnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ertgggin.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2alxvxnot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lszcqvrb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vybfshow.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2yicxaxux.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yknkvtsk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rpzuaurz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fzmsrsij.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2reswjhdz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2sdtkwbdw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2beignscf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ciefldqd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mirngsek.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2glhnbsxt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2djznhyac.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ecgilknd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dszomlll.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kzcrltbf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgolutx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2reuzylbm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mpdgtccd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2snctnvxf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2moebclcw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pykubros.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2paslsfsq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gajifiyw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rpcsyvhc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2myzaxyzt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bkepsjzb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2eourxiqe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hvrejssh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ivrdcgjp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dblgpuru.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ariatgav.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2slubjygo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiswmfcv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ghspbluk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvixvzy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zahgynjk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sszvljqj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jjretpmw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdqlbky.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cbxxyjqt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2humxzhod.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2smlrhpgs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wwittkwm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hamdzzup.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vnrjtoik.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vbqpwquy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdzxcdz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2elnkhoen.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gcgkwraj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrjoflbl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iqkntpcl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2syyrknem.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ibttjmtk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dinbkhkq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2byjntkwp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkgjalxk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oydugvkx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvgubsjk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhgamqfb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yhtdyqrb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2abfvhsuu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2nkoknitn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezgnfkhg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nvjfnphf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dbhqvnnn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cudsazda.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ijpttueq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hjwlazhd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rptqspxm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2prjvahtp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uehfqtwt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rktqmnsg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2blfztkst.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zmodrkfl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tubtbmut.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2geueazhz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2otngizua.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mknekmwd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ugirqdqq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mapjhvax.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gidroeqb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xhkcdrcu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ovkdyyhg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lbfxewle.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2resylnch.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cuulmcud.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2uyabdxss.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytfdjuwj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kptuqlsy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gzuaakud.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2czrcqbnt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2efbbomha.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wediaucj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vpibsthl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nalgzyel.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymwcdsqc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wczwdneg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2hyskjmdp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2agyxjsal.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ecajrvil.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2khlrgrra.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ynnkavtk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vyxnakfl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2auvwrukh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrqtzku.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pxueesyw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2epgkzafr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2uhscacpz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dmymbggz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mrxrfhsk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvumggok.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xgevrdtb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zgfcdicv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jfhggemq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bczxglrv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2tqiglaaf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xdqxzywd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2srqfgnqr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2blzqolkc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pimfxerw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nffjmfjo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxrgiryh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2csxecqos.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zrjgfpqh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnsokod.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgaogubo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xltuoetj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dacypceu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2kpixozwf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dgefsoih.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wpltaozh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qaesbidz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gnrgogkx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rxdfkcxd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zfkculae.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dmlvuikv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ailjvdcq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hutchypw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ezpbooxk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zmhybmzi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ypcmysjd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vbsgiaya.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2regpjtwu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tdseghqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2betbvezz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2iswgwepl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crtgmsqu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdfazgcd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hilvszxp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2euybrwgu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iklpqhqp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jygnjimk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cohbfrsw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2atjomhgj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqnwmdbv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrxuqtyi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gcvhiurr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2oahvxmgo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydltpsit.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sycekiwo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2coxwcmdn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wggfjqly.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uiwlgybh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ekekcvpx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2phhirdry.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ruwjinbe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tfzizkxb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqwordgu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcgdfrfe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cxugzyfc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qjoivnxh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ybfnhzbg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rfpgadlg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gslgofnl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2edgmtsmx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2gwjrxzgt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bgiyptug.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rmveupzd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pbyqpkth.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ixwffbbb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2grghdrnw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2idukvajs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yxwiyahl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jhwwrydo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ekgolptt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ybmaplmw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lslooqdk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yxeqassd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pbfjrnrm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qzsumfzs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wbthqmxp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gwnmmmha.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ahduknis.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qdasavus.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2clnnased.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ifvxonxs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2euwcbsni.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vzjpfmlh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jsgrlazh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wwxgntrr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sfjypzmr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2apforjey.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jkegzdmz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2puyhuqac.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kobmgzso.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdsustq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ektkknue.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2aclewvvs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bkejwebf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dgkwdqup.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hpxyretw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fqtqaufe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dafbsssl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmqgkwll.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jujrbrls.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lmwhmnqe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2prenoxef.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtdfmyfa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnegxher.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qmqnseje.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cqygrqnn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xiiaarns.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nqskpopu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fvcgpxwm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2onhhwkbk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2crzjjqwd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ktuclyre.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lmngikjp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vsxrrloh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nczzuawb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ubwgtyss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gvxjxnpm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jrsiumoh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2awsqrkxf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2irmbgmbz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2iozmjger.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ylmgojlk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ednlzmdz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bfxbnttg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2whqiizah.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ipyrwmia.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tlkiqayv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qjelfgnk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ltbeffvv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kdaqocpo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2prqamnsy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qikqzutr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tnwepbkr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fqxulclr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pwocfnol.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cusqplgx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2qhtlymby.html


<!-- 参考信息 -->