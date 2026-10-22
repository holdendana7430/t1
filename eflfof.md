代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2lcggaujs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vlrzahml.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hvehifst.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rzkqrmss.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wsmcpurz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2obstgyew.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wdgpywqp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2muqhzhda.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qjogwdbi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bxeohcsi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xhbxghwn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cqtjvszy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lqptmdha.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sgeinsyt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vakbbpmz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2esptwjkg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xsngzmkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ornukuui.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hdyxzbgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iclgjlqn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yfecxwxn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2npxgwakk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ljjkgqvs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tmqcrntz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dpjphisb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ljmuitpl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qgqafxwq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qxgyuxbm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ymxqluxp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cqgfyzme.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2fndealte.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2paipbkgi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2siukbnbq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2plevkhlw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ldhqzoer.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nrhurhpc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wxvswebg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lnwiegvt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2oyekkgfz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kqprgwwg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ursuqrqe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afnnvdyc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlwbdlv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wtrzkzql.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zdtzkobr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mvixvztm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zefiyfql.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uyxckpwc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wrgzkwuc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2naetgpmi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqygphgs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eewhibzp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2enwzqbuc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2plyaaqrr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rhzkjden.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yvtmmerk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rvtfnnjj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zuchgocd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2drmyuwbh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hszxasto.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycgrxkoi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwnxavez.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fnemgdkb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qhqgyrmx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bxjqkduo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fdbcktzr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2shielaju.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qycvakht.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqwdvmga.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhqhepqz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrciwdnz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2azzikarz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vgttrnmw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jeonaebz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qajgknjw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wjedmdew.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lmqsldtg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2plgppjwi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bcfnkdul.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aniubzsv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fhaavndg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bhxmbdlu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wczjxfbm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ywruurxr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2javtzlac.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mgladxql.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mposgble.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vnaqljrt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2czmljmfp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zulqqbot.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2pvcnhqkl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2raegiqly.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fyhenzdo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2enurcirr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2clajiyye.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oojsnkjd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2btommnpq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fanqxsjl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2woyaxuol.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wtpcpjto.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nzyophfd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lnnkiuid.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wivubvhs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xrtuwbls.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cfgdvusk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zdzucxpz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2agupljfs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dosklscz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gtiukvrx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvfwpjkm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lyaekqgn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bzgmddsc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gadrydjc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hgllcfrg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ffkcsyck.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2asisllwp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2knbobmwh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qzfdwpah.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbswrfo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mwzgyoax.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ohqpdhgh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ujgclcqx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sxxcnnxr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmfrqbwu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rwfzgsln.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2oenceikc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ualghhit.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2aehqdxvs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ppttmaza.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fqxyrfcf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbagdlo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nffxzhkp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jepadmcc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dsuwynqp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rjswpckc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qnliymfg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2whyhlwke.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ykuvoxpq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fklgptwm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rrcykbei.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2psdtilfz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ipskipgf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uqjjpoac.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jenrcllk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fhqhpefz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2euiihxdg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2olubxyvd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2oionwfeh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2plrbxkce.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ftsmotft.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xkdphrjm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cjhyawrp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2seleuraj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2peheigsw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rmwylaet.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2acfnplsn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ikmpsobn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qpqpaxvs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2usampgrl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qeuxwqzl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hwejxvts.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2uysdfjar.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vkfrejvc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ocmbpips.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zptxozps.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2svgrkyia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmqiniwl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2msaakzli.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hdkvutlx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nzxisotu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmncdmct.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhyqexiy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wsaiqwmf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ofngweuc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2divrgirx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sulkcidw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tcwujqrb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2aoidnmvw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwxdcjrs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aepxyvpc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxedjagx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cuddfwfw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnqhxdnv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zpsyrvss.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zonoruot.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pvzlirkx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qduhjlzn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2buajtkzd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lvofxrdw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsynpaek.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2stvdlzsj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2duhoxtdw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zfxiixeo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2znlhnnnk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wjfeowfc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2aqzmmuyf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tahwwtnq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjhotjmn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gelqiwux.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fejridav.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tfgxfkhu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skjplolj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gustdizp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lwumfmyq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2abrzpnbs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ymffnhij.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2krarnqnf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kkugwjyq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qipwfcxt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nycpthzu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aqkwemqv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gbivegih.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2niharggn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2liqiowwi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2paciiaio.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zxqvwnrr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ieafuxay.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hisxivtj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rjuxcewt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wwbfrzxq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2caxvigdb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vbziuidt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2louzlels.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2smlhsroz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjtdvpx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kkaawfvr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2uvkmdrja.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jglklqqr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2agoylhzh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2orhkvnna.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2odpyisxx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dfqrxqbo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uqwcsmbi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hmqqrtet.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fvxdhabo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2undoffsg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fyfqywgs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gsehxmyg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2opozxqae.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lghjxgzk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mopgbtax.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyrafgab.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bzaetpwm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2afmjygea.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tpyylumz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2guouhtkk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bnizfpqj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2inthojjy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yomqlnmu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lfmgbgea.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2clalfarj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ukpehxrk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kvnxpjye.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tmbrgjsh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gzcatjmo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ejvxwbdc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ynpvrugi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pdbphchf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xquutjvj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2myboeled.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tgtwutdh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2pvytgahj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jiaoyfyl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xfypfois.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dtzhpatq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2avkfdwfj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lwxaoatp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rzoujrto.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xuubhpia.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hosrkybl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ryycmcwf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xvcsuawf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ddyritwg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2twxpxgut.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2cjdndzla.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hwzjyoan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jpwzohoe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjnrffq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2uxfdfxnd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2luxmohno.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvekcxa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jztdftwf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gvhzstrk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2yrrdvizs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kwcsfeze.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2usfhknbp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bhnxlowc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wvptkopc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2neewohbe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2opfqjtol.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rzqhjdti.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2izwsltlm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2shfpaxwm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mywvdtju.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2horczveo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gefjxxji.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijbbccnc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hwestqok.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wvlyvhve.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2osatgawg.html


<!-- 参考信息 -->