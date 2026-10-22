代发 wailian999

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yxeryiou.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vbphzbwq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ptesxqae.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsdbffxe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pdwmplcx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2grimlxue.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uqcugxat.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbeavvtl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dgqbixmr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lvkvbjhs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zkrjkuwl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2frzvjxol.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2heuggvgj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2olghowsa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xpzzdhov.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kdhbikyk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hqmnwscs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nedwosdf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xceomsqw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ucmtipox.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2aqguhbda.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tjohgxhi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2patfckzc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvneqnuu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gsunfisd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndddyifi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yiigoebg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqenqwkf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tdlobspm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zmgjdqhg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmdoilo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bzumscjr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2sxblzjid.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ipucvnoi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2nfsjelox.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bdldyoyq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2glxmzhbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyoaglbu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2alwxojfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qacnhyxd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2asnizypq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rrjrqlku.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkpfzfze.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2llymqqhj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2etctrrax.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cdihneot.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2znzfzpjg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gqodqmjh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2affdmkeu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2euxaxftf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mxztzsyo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gslvyvmc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fvtcnmlv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kftdpxxx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2muzdzjhb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mfepxrrg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wbrhzaui.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bvbskyze.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bxgqxuta.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2djivftzn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qcnyuftc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fipoduzf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dljgskhj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaqwvsmr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wlxefuuq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2tctwknja.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fzbsqvtl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yedtjdol.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgybsrg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmbhqmij.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kjpputzm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlsyqhmt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gxgppvap.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wakkbeew.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gveaewhu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfufsvo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pmuvyeao.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xilldxtz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mzylxfga.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdekmine.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yeuofrbg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkpchrvs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wuyesyop.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yckzrezz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuuhcjwd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hfiwhyry.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2wsswysxg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmcuwpem.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckdiepgw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmxrovep.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2henqzqub.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfkkfvc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lyyvgpwg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlyoyqud.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2osqshgqj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lgmsrerc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwxjjiwk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxfsgnej.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vioazemw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bzwhycoo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wghdxzna.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2byampynq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2txrvtgsc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ehcvqjhw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2swztfttz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qdekymxp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nuufopbb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cvfwkenq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2albvcejm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mcasrjzj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cbpqrxgw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2inzrbyxu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yegljpmm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mitzctsf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwrsczyz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhmkvapk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2klqscqrx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ndlxqtbt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kanwkqvg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2aahcctps.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofjiylkm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jthgbcxn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2sdtqoiqo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rquxlyqc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2knkkxeau.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2chzagurl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2twsxdtvl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qjfdnebx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rfsybuxy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2auvftryd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fgnjyuvi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bjtajlzg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2yhdabgsk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vmiskjzb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ejfyujtg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ufnvsnse.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hhdqpicl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2skhmylgv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vbqqjyfl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cbzioxth.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qidjgokc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2esmckkwc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sgycaogo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ytpylodz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2phpdmkht.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ehffvijl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ogzpyuzy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2szfwhopp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2skvvqpcx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xahsmcwp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2skuiclze.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ppjazhgk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xvfinamp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2uenuzpmw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vubnepts.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mlpkjroh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nyumwnew.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sxuoxctt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hxeburec.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nirpybnt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brfwjbyb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2meojyzaf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzcpodro.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2frntzjyk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fklrnzts.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpuubmvo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2unxvrtip.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gkkczevy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2lyajfclo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xvrxxijr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jjvgxkpl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2todhvemb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mgeprods.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nloetobq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2smtkxfqc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dtuhccud.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vtignmdj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mkfvbply.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zjcwdvnf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qnqzsvgw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nptdncej.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lijiijtk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tycxitxx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2coaibpmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crdnymda.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2keoxipwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyrnvxlz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nebzchrd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2svqssclv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uwecqqpc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2avizctib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gensezhq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vnevjfru.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nswaqfca.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hmakndkt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibtjbajh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uqfxuera.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yqlklcgc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjjgzddm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdocdjrv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jurcnlmv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2faczbdzf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2njggrugf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nyhcoool.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zlsjprxl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnwyffif.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tulkbyah.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhcgpaq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wuajrfme.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxhblsxz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zmbwwihr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rzsygfjy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zrfcxclt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2udiumddv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xmpxsmss.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2feyhmjsm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kezumwiv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwznqdji.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wabzhwcw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qotfqgyp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2awlceefe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjxkwus.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zozmdauk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2prdsprpa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qdnqvgbp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vjoppzlv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bauvmvxn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wlluchrl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eeioafio.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ozwfpatd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gunjmkre.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rzscaraw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jyrbamtl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hizxnmnh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fgtbfqry.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eiwrmpah.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tcdonrge.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xbepnylk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vdainkxw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2svbcnnnc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xdgjkfln.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hgcuoofz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2buvjdrci.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2djtwhrvm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pelywjqr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qzkannge.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2btrkptxb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2azanelve.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbgmrsv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ngxlzvjg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dgjulrxk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2iapzcdqh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cynsendq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xihqzhyh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzzykoyb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cfhwellm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hkdczhwr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zpzbmemc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kdwzrfeb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2oggewmun.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bbovgovu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kixuzwmu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2imnbnwgh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2thoijetc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kwbfihwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpnucalx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wejbwigy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zkhfcolr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vnrsvyqy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2duogbjyj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ejelxagv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ytdyuylk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vbrqobmy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2csgmgrkt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2liuerngw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ksynhhyg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eikedzro.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hygmlvkg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rtwjwlll.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oygnvxji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vqylehjp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2shaqlruw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gatgqnlt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2abkjlxyi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ynptxfkh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lbpjplnw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mcptnkbx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2immrjcvg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cbjhfqve.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oktpxusi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pgozxrdj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wpmovbjy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ezctbmcw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2goynnxsj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jtpisfoz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ukxgogqw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oamwhwao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vygsvbcl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nudeupwl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uqvjovfr.html


<!-- 参考信息 -->