代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2hzmozvap.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2axsogkhz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2gjqkyhsr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2deofzjdt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2dcfxloyy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2evdkbxjo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2eipmvzvf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hsexvkal.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2svuvmndi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yesedpdn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2lknzrbjd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rnmlhxyw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xczcitxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrsadwmz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2sstbbkhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2illiachx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kvnylxwc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2sjmutyvy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eftmqsht.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xexozymq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tediivoy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jpgpjlqv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jkogqfjb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lhatbitb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xkhndpix.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vbxffqig.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ktzxtqkd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucnocezg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2veckzdfy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pttuepco.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ryehwjjr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mopyqkbw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2bqozcvlq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vheuynmb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2odawbibq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vjcbjbot.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dtuwoppp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wnkagrsv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2goicoowh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iybmehry.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ddojqjrc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sngukaqs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ainuwdmk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nbilmirb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lawcvgak.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxygrbtc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cvycjsbq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fxgjyiut.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zsxioafy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2soyhfevy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uqqwjqrp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eakvefpc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yadseqos.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eoleptoq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vglvrysw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qinugxrf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nohchlsm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lxnrvjpw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wpbfetoo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2nkjjbzte.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzbghczn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gvusqqgd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qsavturp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjkxhvc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2svatdnkp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vxilmpcu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvtkbapz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ezdkicbq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2htzzfpkh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqdypqo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2osbhsrbi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kkweduhk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfmqosa.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yevqyuya.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjhxwhop.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2epbpvrby.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ivfmzhwp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fuavsjmi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhjnfdvl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2azuantim.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gfcbfruj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2syfxrjwv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yuftikgi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nnlerwlb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wpswhpnp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bfdbmjmg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fyjhflnq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hsxlsmsj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2edmesliu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uslbgprg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hrzwdemk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdtjiirt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2agktxlot.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ivanfkfn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cjetbwlb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rpvbxcsy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxhneadv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hoktetft.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2drykswae.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nxitircd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cvpqwvrt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ykjfyzmf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kysgucmv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wkkbtsyt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gbthejla.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2slihjrdl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2unabapdf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fbmbnfvp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gcgbfypc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2llvomsqt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gumobfzu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2oqfvhbhl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zfchvsgt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jettgbam.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zppznbmy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bwqdmefw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nzhwjdts.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qzlsexer.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rpvmhzfo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvtxlcyt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qrdosmon.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dexmkjiq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ghhucwbh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2sfaeglyv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vmckomtb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qtfcrvdz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ywilhcyh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hmqyvkkn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fqnlprjs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xelgpbiq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lvakgktj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ngwxvhtp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2icxuhklh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jhzikzxp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fmguxbvc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qkhsqlqs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tzrttwhr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2frmtwrub.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dglkyfhm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iagubmmd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwxdfnw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxcdrcaw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hmxtwuvj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2axrgelgn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fwmihsle.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uqfjlldw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mkbghoyw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qxvpjvbr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jgvsepcq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fkvqzvzv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dbirlcht.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gnbkcpqf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ozwdnopy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rchphrxd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2anxeczrs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bvvbhnaz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bfspmefq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrptnwv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2umhbkrsb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lfcpdfyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhigiijz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kiufaowm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwfxyfda.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2txsvscgb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lmjghhce.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tntvgqbt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2inkphtsk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uryxwfia.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dexkeolk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fmioizyo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2aklulfsf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dtmzfmrl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhanyepp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mlfvaybr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2huejfcbf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kjaneedk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgcpmbjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yumrqgqp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2oiboncqp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hzecczxg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pjkvfxbg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2snmrvice.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ovkunzge.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwvdozct.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cqievrjy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lmiiksil.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmeerpeb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wuupfpvv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mezrfylp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gshdcfgg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfmrrcjl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qoxvvrqz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jfcbyhex.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxuswxwv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2cotgmcst.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2knrcinxq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvdebatd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxefcrft.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2klldowvq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2iylxgnpd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yphwomyo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nskvieug.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2brotmapn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ckdhhcht.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kxhiragm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eeuncubj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rbiabwif.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rejiiexa.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vdozqvcl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iyauneqs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2czcqurgj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pepcsyrg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rxyqizms.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vrbzjpvp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fougvqfw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kgkvslcy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rzadsuns.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ksunjhvl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2fvjedqpn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qdjfnzps.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dueltxoe.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2eszwhndr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbipsorn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2auldrzmd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mskvpotm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nyeyzyle.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cwthmzmj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ynrrzsod.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wpaozosa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tymdtvta.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzlidiqc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xnokuyav.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2cgbibtzl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2caluikik.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ryggqsfd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2nthsphut.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ceyxlofz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gimfqoge.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2iubeefyw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gvieobdk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwkechhl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gtqadrns.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qsyxeqia.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wtrcfcrf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qtkgmclw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zugqhakj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2devimgxe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2govamulq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ttgswzvg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wtgwkaqa.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jigvawwk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2umntxvzx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gnlljuvb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wziwsdrn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2yymndipp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kxbryrhh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rfludhba.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cglzocst.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2tobcmygb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xietnaqd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lbugouag.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hoefurny.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jedlzphw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tztrztrd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2phqbtrxd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zvmwrplu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2eqvmtcbw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2aoqlxgso.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qacnulwy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ydmamogz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qsqzbrzn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2azfjxdfk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2oqrhvjlg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uapkfzsy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gtnseglp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cgjzuddy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kadrcfxr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jrpxxyob.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gvrkllfk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ododsvfd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2quymugxy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2snpkejep.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vkcurjut.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vkrrdimu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jjmmjgfs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ktgzzmui.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmzdzhg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pdmoylso.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2noyjnquj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgmerpsl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sinlmupl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fwxeprpk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2knxbmlog.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prbddtxm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pasfjmhy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jptfjsiy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ntkytvfi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2osygkroa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hjspjxjs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2igccdlsx.html


<!-- 参考信息 -->