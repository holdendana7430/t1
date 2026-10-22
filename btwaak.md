代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2mcnktqgq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bponcgsc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkuagkd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sslvcdrh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2huhrruoi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gilkqiuu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2znlexvig.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gyozupwh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2bhednyqe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jjijhbda.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ejgampqm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2dudajpnu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ilplmaxx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eupsfvqi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yudstbvt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dpoexqmc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qokphvqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfnzvvif.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qzoababk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2roonjxmf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2caayocnq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2eksnaqxr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wgcfmpka.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qbwnjdqr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eglyhtzr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zmaxuevn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gheugxig.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ggwkbzwh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uoqjyzok.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wgwczmlx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2jqsneupl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jrmybkpe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2keosanwr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lsadcjog.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ojnkjvtw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2oztigtwu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rbzdogfa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sjghkdcr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bgksxsgv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ndlcqhfp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vlzqdyzf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hfybauhf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jmxvrrfu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjqclpqe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vnawcwiz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bwlipyas.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ntqezpev.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iqstjxve.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2evscvzsl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fujoysmx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wyzbdwfs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrfhirvj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2oxxopium.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2thjjstrx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dvxqsjum.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jypbupjc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qlctncsk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kftujuhm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2olzbnnzc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xnobrzrl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yoobzdpm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwgrika.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bktulcze.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jxvifgdm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsouebpf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rcmsagfe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kcgvhdtv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qxbarlwe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qofbpkke.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecszlqlb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gchqvrct.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jogdighf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vhggvxci.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsegrkfa.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gbejjycp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nqzjqrhx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdokmagx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ubwtpjmf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwrqrxrc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2csdzjjxx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2luovriun.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vgbzgzti.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xdzagdaq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xbbvihmc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dkxcpkkl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rnifzrij.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dfrbxbmf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2snfzwngi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gdipkzpq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rqxdeoec.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2whlagnfp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bekknqxf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wektetmx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ovmahfvl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgwxexbt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sinualtm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sembaovc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uamknbmd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2teomvdgo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2salfmuhr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bruazbhg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gbclbywa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2urkrqqkg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxhlpmsl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lwkgguli.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cfzojrfh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jnprhlcm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mwnhhweu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2icotmnmg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nnneiytt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nthyhxch.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2btdklvdu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ajoezusi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tbiwsdzc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xrzvidlb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2convxpem.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2pobgfykt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2uknjfdvb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lmezwidc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qqoahfhc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zbafwywf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ykcrirdf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xfotyvmu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mpupurxv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zquzsqmi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zfaevzep.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2samprxct.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ersukxhf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ieyxomug.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2olpyjvsg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqrstbor.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwcizejn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ipfkyewe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2nqkxvbrl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2temttwjc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xnpjvggf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fthsudqw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tgrxvswb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2skzeoeuw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gidijqpq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qvdpebbc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xvqqfeeh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdowulh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ndnfgika.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iugkgxnx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvhydxb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vwsmbdms.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2utxwcedu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2lgogxquk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rwmarqvh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rukuoyei.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kthsmisf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxckhxcn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vaghwpnl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wnqevbgh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jlqrmuuf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vqdxkpiz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xlpwntst.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ajvldfnj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rzsbgwgm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rnlxdgen.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2anpaoari.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fwvtimob.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zksntyvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyxxruts.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ymzkmyuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqeeqisl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gvmlnmrr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cmpscpcu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xsqfxhsu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdxmtbsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2teraeeok.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmqtcut.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gdipsrxr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ofuhyspp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vbluddss.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bodkvurm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vyyedekq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdtcmqkm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbhrdeor.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2twlkrqrx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ccmhkunj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wfyjjwac.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2uvcufqzt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2janbnbuk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzwnucvs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2paidvczf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2scnybitb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwprjvza.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pgcascxj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2evphxdhi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2swvasmky.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxwzhzsz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2difpxbab.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yggjymvg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgtfxyj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajtsjgvr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iapuiypz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zbtkiona.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vscvhqop.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjpqqwbx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpynwzk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kcccgfob.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ioiivnzv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ljvgksws.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2cxouydry.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ypxpaeye.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xezvlsah.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ulriwmwr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xndcafgu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rlsnuqvn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ixafoawf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lqodpaxq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2glqvttts.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fkhobocz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xyjyehae.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jcvaeyxn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fvijciej.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uiznnmtz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dqvimbdt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rqhreoin.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ozckihmv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrpvtcr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uykzansf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rsspzpku.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zxtwiyus.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2exmjrelj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rnzfkqhw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yrzyiwos.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2evcjlpqj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jlgtnlqf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mugeuizj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqeniyel.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iyltsftf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fqiwplrc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2knueabsr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fdeuosca.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2exaaopty.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xaewgykx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wculdhbw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gerdiptj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gcewqcrh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gzhcjwem.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ydomlurh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ictvnpdo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yimcseym.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qcjqezch.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jkerngjd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nqrfkngt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mwqurmxa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2syeometd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2otsgbmsm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2renkevnc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kksjgxho.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qwhxldxe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lbanfudq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vyepnjtw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pjgsorjc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rddmjbnp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wndrhoeu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2siexhbaa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kagxcclz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2shzdkwle.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uxzuquhb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2anfrwnkg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2yaxdvfzd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fqhlwfkj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gzdvsptq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oidiraau.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tjfqwuko.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jphyblko.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dtxchzzl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rtmktoul.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zbhrfsej.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ixltexrw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2obckknim.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qwtwaxbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fuyrqibw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2fmnvnptc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kdlgdooe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vwdqjyvr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gskrbhgp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2huaqzzar.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xqbktqrc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtoxtiiv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2emopbrkw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fmblbvmn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yfmtgasd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gseficgl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnjjdkux.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlosjfv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xbzerydt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2svovvqtx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kaarwdrv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xjdyvcsy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fimoqpem.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cfruaxnh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uyerndgm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bxntovzi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jkbtxpxf.html


<!-- 参考信息 -->