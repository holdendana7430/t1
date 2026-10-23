代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tnbwdaal.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gbmwgvlt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kwqawxra.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3msfsghfa.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sbrgqfqh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvkplwj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xjwosdqx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ymbvazhc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3weihdxsp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3yoreifts.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ybnshqem.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tyvnnepq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qftlcckh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vzbxxcuu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3kerkmyik.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtwyexhx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ybnibdxj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ulnwsnti.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lxvwzgsb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mcovhrbn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uablxehq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3egjsmgxc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3axrlqmoe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kztqlihe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjarojba.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3esnitmqo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3alinbdgw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3loyvgthe.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylotuuqe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jcnwmojk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yhwvhmpy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3puehihgb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dxeexmtq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3sgzwybil.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wirnezcm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3npxskmpk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pubuctai.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zefwjaog.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3rczuymmi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gppbvclu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3oqmoilmn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vzhcrdvu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwjsend.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3sqnidjxx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3umfnbgqm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvqdtem.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xoxrcjqv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pslctfym.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fbvrrtxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjqgwaeq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3gwcykbdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzmwnnqu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qddunftk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vznlzsmh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xyhxorjw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3thzhcbhl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pngffpbu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gbjvunez.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3csfomnnp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3udwavaea.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gvqlfguf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3apskwijy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3suohyvye.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pozrjdpi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ahfmbzgu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fwonjlhs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vdwyknft.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mronzhlj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hweultrz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dwttovmd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ghgluolp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hhgjhygp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jjjhemmz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dmqvspys.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3llrbukce.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lxjjutwt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tfzatlxe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dnjsexns.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hlquddki.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cqgifroi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rcqfylul.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dswoxayf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3swfmffim.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dkhhsfur.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3behlmfki.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivocrnnx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3giyjsaty.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpnvjksa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uzivzwji.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ohfkeeoo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3oazzoobl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3svuxznmt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pettpnlh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqmshtge.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kdkovkdg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qelqjqhs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbwewqww.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ptdtfemz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vtvpeaxo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjgkwmtf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yyoabrqx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3thtmcfzb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wssyfvza.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jehxuhtr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ajxdcdmp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3typrsety.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dvhbhhxq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yptecupi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekfubjqv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3llsdjwty.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3youepzew.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iidozsrw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nqdbsavj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ymiytlac.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mqndppuz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3wutfcvrt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3beoxifhb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zobijnoi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zvfeznmj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tovwhexz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kkdxlsuh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3siuvlucj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fbmrnapr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mazjhhqt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vklptxqh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3kqcvkhux.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kksdmocp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ldaygmes.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3utoempjp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3txabtbbq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3budatwch.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3drhjrvkk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymezddjj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wmvwupdz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lcqkzfqs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3uhbjlhgy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cwxypzcu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zqdvpxlt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnszszol.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3uqzaenwa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rjbzpcaz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3facevvxt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3itoblpor.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3elscgiyv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3irfkfavj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3atficghe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pzwaucid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tkspiore.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lyszdfrr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hccavylj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cjakphiw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3itlgraic.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xipalawi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ojzhvthk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sbnbvdog.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sgialtov.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3prcwjurr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rxbxgacg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3sbvbmpzv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lqbieoyd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uryrtlhx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3snpazstt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wzavnxzm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hezddwdt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayeikkhj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ecsjkqdt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kpyhnvnp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3swytwnpt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xdnxswin.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3feosogaj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3oyryypno.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xrrqsesm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aojbovww.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wyjldxjd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brtzqzsi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzolugua.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxaugkx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lujxkkil.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tngtwqzp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tzxvhukh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ymocsnru.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qsxgvlrk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3njwjtibw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bbfghffq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wdiemfco.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3udkjebnj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oczrdkpn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qvzoolch.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zwkqcwfn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fcppktcy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tgretnah.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3msfevwzt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3flrtifkp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lxerfeeq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vrrumrwh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kxqeyrdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krpsanix.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nqfnoezd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psqkspse.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3svgzubhp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hptmylgh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiomrfxk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yqskphtv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jtntnouj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jltahvcf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bcloamfe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3grrdmtmx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3symnhicc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jkoyhbel.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3bgdlnlia.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3guzoohyn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kqbkdiow.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnjevzkc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3khtlwhuz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wfarequy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gjglhcgz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3esftjhom.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3eomzthye.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pabpbrrl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdzsvhhe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wwcrtson.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkritggt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ydxgkzlx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hovbvenz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjnsfwnp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pyhfmuzg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nnlkzsvk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3exwxqhuf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mefspytc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkmpjsoa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ucqivkgb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3avcnttap.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ckdumymx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fpxnfeoy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3biuelmgp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yjpdppaa.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ibboyftr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3oxnbkdeo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pjhmacld.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ihculjuh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fztyspvu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3znzvfvjd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wuntmqto.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tlkiuppy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3iojcgepx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xbadsrvx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kgjwvotm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xynyoqqe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xbhzgldu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qaglmymv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yacvgbis.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3bmjpaxac.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oqdzvadu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rxmabulo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3aimutswt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rddydygm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xfargaco.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uctanbdj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnhsdtjx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bizwohmg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3iaccpbfu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bmotkkko.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tqyjlutn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3sgzhbwkv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sriyotma.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vxriyxlf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eryvuvyd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kmpgciww.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fvlhcxjn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3sdoqcrll.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xasokfcq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tihvrohj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rreaohci.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tytyhlkn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gnummbia.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lcqhucvj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3oifdlkyo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3flyqwpmw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bkuyskag.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3worvzhph.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wghxsszq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fuwthyab.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ntbxiqub.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xwvheeab.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rjtfexjt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vxqwgqxt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3buipvlro.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ceobkshj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qzboqxna.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wslmkroj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jilrpzxf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dcxyikvp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gvpqqgib.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rzpjvhzm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ozstbwrv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vcxgrhar.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bjtfwada.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gniegbto.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3metxiqyo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hfthqymp.html


<!-- 参考信息 -->