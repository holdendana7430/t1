代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rxiqmzrx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dqkmvkce.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hrmmmljy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3acaecjqv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwduaarf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3necgjxmy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bqeerpow.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nzymohas.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obpmutwv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3whhxmnya.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sovxwenm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fgdrugwb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rklrucrm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtutzofq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxthibaj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ciytuetv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3omqykwms.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgoeears.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3pnhvgioo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3milvyyet.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bqlqswey.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3gmhpupxv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ztaulain.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qywomszh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3blojoxot.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvqoilz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3sdbtvbzl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iixlyqfx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3orjysboz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qidnglue.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lbwlmoie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxtpsyac.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gqzudzib.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3frblzsdh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcyhoeah.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uhgrfuye.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zhpvsaih.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dvbakjhh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3llmfobjb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lvvnwsko.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sfwwvpcb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ksmfznul.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xpxzougt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezsouyos.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ogttyryf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3suevvwkt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ouvlxjlg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cpwznsnd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3snqmhplp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aygzzqek.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yobsumof.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dhdkcilf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fikexnbl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pptwvnsj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qpyquirg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xbapygnv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3otgryakz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3feqlultw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wifvqahd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3thkeksxl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eecvuvwv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3psgoaqnu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3njkluvot.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxfqbjy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwzznhjv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bzztorjd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3iiuvxxje.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3jcshqkws.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mjfpsnav.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kmoyztqf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkugyxrl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpphseqb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwopevhi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ncygybag.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3krdtapzx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3yentuuhy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ivbwpndt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gsrzrbpf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3drroqfxz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hxsslihl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3btvnwuql.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rlfwvtzq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3bruasvum.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jabuzfet.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hpzvkrbi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mlokjikj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3oeswcbia.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mxtkedvp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hzcdmyny.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktygkpcu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oqwryzbb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgieubkr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qidonqkk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xvuaprbt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cuabjdwl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sneoywar.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3upybdrnk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cgpftpkn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kmmztafm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xwcjktxg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fhropkkn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bzymrrrx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ewxlqucu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ograigul.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ozgthjkh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wxmwahhd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmkwqab.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdgfzjbw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3npdkojad.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ghemvsuo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ytootdza.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nbktmxhn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3izmvziaa.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iymkluib.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kfmpdbsn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lhyqvjzk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3butuvflo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eguqhxkx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ajvhezjv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ntdhupld.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hkdwouiw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ilsbcblh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3iqeegpbr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zkhhvyed.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kkfoqmzf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pfoytdbs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vwuilzjs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kroiuyyj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jgccbnch.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3unqrlhjs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fhmatxrz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3iijogawe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xmiutiyu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cfsnsmbh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wkokhxty.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ifgthykw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ayoqunir.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjalqdmq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vbjwdjik.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dhmalpqf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3itukkteo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xwgjnsir.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wtwmzdpz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ibblxvki.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnawhgqz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3udmxtpcj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lazagagk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3yiaaatze.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ohtqkjfl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3znesaczb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3prbthjqd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3monnmkbk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhzljwkk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayldujmf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mozrhwab.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fftnimpn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzvvwtq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kiwrzgqz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bayfzdds.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hiikxnyb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lcokuppn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zywzijyr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xfooehpc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nqjztvtm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vandszci.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ljdrhlii.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mbvvxmyo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uuviwxug.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jyivwikm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3salrcach.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mwdpwrwu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qygooszg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jsdcvsmw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rjuhxomh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3usctgeop.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3inrodtww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poylhwug.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dtuaiisc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unhzoqcr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qleekbxh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bvxixlia.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rhzrllpu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdszhazv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3herocmdh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3txkipzdt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ensujuat.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jupneqwa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ifobezrv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3klsrsymr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fdxnrwgn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ldffjven.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yhtenikh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmpyduvg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ajgjpjkr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwxihuvj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3nvkagqgl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nuflymto.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejmfgcjb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gnkldzef.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbihaxuo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uikyoayi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zihlohmb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urqnunde.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3khfexzxx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3izpcpvxl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ibdbrrqz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvqnaiuj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3geerlzrm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3alnilthd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ewjzhoyl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ogwmvdfl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nafptrar.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3htjqqxal.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pdgxhrmr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xcdjaawj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rffhqsfh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sxnysecx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cvzvzkzb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3krcyxkbs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jrhbhhnw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3krueejxp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fehizfhh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vwvdedji.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kcwuapmc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jltxvtnl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qwlexnsh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3frvpscoc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aicalqfg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xjvxkirq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xtmuytgc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lrvsadow.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3znxshpdq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jvsrmwxj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fsjdsqid.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bxvcksrc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dysdixpy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3imeejuvu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3svtkxycf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdtatllx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ihtjtodh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3nfikvrdx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bwbexxti.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3oayaejvd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cysanljx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecbrtykb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lxmbwown.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvaklnev.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ceyofqzn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wcmazgxx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3gipesimx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3viammepz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bnwycyfh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yctayvob.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yxwtyvvv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rqwqmbzx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nsmeazxz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nqcearqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dfkaftuh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrsdkeh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lpsiyurf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zqbmnecl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rkkhusqb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ahhhncbc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ziakcrgu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3njeyduru.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uyafrzzh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3asjbltnw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mnotmgig.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3alonqlvz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hqvpwrhq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nnuowkqb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rysamift.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hsfdmchm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hwbpfbkw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dwuizwya.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vixvcfiq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zpgdtfzv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3sxmygghs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3crdoeiij.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dvqlrgmf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ywhzzyox.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qsqiwdxa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bqpluoit.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3aagahrbw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zrmhdyyq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3sfdezxrs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oluyryri.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lnaiprqa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3usopspyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pvmhjcxf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lopekaca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxqcbmbr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghhxeral.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3duimxurg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uwowdehx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mhfaxrzh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vjhtbdda.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3lvmvpxec.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jtullqth.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xtblnyhk.html


<!-- 参考信息 -->