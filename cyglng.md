代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rabywnuz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kgkodaht.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nkyzyjsw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ypyuscxc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ucwywrff.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hvacfukm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2mrenppex.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2imwgjqws.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dnenfirr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfryptp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pilisrrl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kuctrlrh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vdabjgym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxxdootw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jjwshcvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfzwlbdu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uvlhkpjc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vlcmvxwp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vxnxbndf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bbyaoawe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gjudkqmf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2brurukok.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vsjszqxz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2psvzaezu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iyvjnvoj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2dabhcuxa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ubdqepuj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmtttnrg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xepyxave.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bkpwmdcd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2akiorejb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hflxszvb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2slurgwxz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2puccxbxo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2uxwefoax.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hzrnhvuv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kntuqmdz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hoevlper.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kujvvrpy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cqkwpzrs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ngrarajg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qmzoiqxn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ksovuzat.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fxpqszxw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2swhgnbpi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nairiwhs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bykfcwex.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgoskeim.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmnuejc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xjumiefb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gcvcjykz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2winqbjts.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2muaqliun.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2scpvpvsc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2iduemlkv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnqumtoo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2skpvjfwf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvwfnlnw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2pwnlefmw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2kekomjyt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2srpkgmdf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vwqwxbtp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pitznqzc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2puxzxttu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2upmjigcz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyvmkajp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uxsmxxmd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qosqdwmm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rccwdynd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2quzyzfzf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qcboukfw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ufunbtts.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uupyqosk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2exnwcsnp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwhvaxae.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2apathmog.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jivzjuvi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wwconfzy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnqcidvh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2krroyieh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rokgfxwl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wyoltpin.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ilwaigkf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xhmbzcdh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmwqgrt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2drxcttua.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2azkloxkj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jhljwpes.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2nwyizwqo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tsqnolmr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxdgevgu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hldhiqbs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzekkxld.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaayesev.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxnttjhc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nriejgpv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2seidafaz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2urkdkyxb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2suydxqne.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fofyowzu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vjkwlfkp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jqkhnbnx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qjburrrl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rxpqorvf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xvolgqva.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2grrgjmah.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2veapdaiy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ozizdvzg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mdfyriio.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fpdjufse.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wpucfsij.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mscnnqum.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ybgmurnt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2syassrau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qvrrctiu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jcvjpqfu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gonpzbwg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2takfvmod.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2efmgpwcd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lsqahdol.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgrkqnuk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcwzpuju.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2onrrqgmp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xomzndbj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2taubiuen.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bdemalzq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2buewgqnn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqmwryv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ihfjcvlr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xrtshqfe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lvwpnffo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yprirqaw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2yyerremu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ybtimsfz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xvpxhziu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xxsqdbrp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwykocs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ztvuatsu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zpduwqcw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sabtasst.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqlpeyrb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tccbllkv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2egnqxrqs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lchpathe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vynqkica.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yaqfwfzr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yefrwwjk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mkwjvmvc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wmnxglys.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fbztgoab.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lopapdkx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hkjqivqh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2thhobtrd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2azldknql.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fjucqeqc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lftdxrbr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2glfnuvdx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ytglazyp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ebtxfpju.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nqqnivfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifbafzen.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kanxzubt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rehvtras.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wszeoimf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oxnxypnq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zowupcmr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpvydwxn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtjomysy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tavcylxh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2syiukoyc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mfjompha.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycazfqfr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fojsbgwt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2aifzdwxw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rokufswb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkllgfcb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chrmpkew.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2smojgkwi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kenlrlne.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2eszkecoo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jnscaonb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vbewzpnv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vptxjtvs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2srzhevxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ojdjlmlc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqpftgae.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifnocpoe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wojuezqa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2movnxnaw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qsevfsgl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2exufyaso.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wrwsybnw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2prgszybp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zyixddha.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kuvmxjkd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pgzpyfye.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jbvehdxf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgluqls.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zeafbfri.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zbpwksdc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ogtfmeox.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2fjchipku.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2knokyvkf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xxwuwhql.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pahmebro.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yzghaxng.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ifpzmuda.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fgwyeaxu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ihnqpfug.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nwdarptn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kdweqsyu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ridlkdpx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2boqbqdbg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2embcibwt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2cyimuulr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vvcmvajp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dlmzalqe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hmsyppaa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sealcjei.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2srigdpij.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2azcdozaq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2yzbuluwx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vfhqpsaw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kpnnkikt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2niajbcoj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uxjjjbej.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mpanefuq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2uwduuglu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtotcbm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xcqsfkac.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ovznhqis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mwiiysal.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2viyjhxqy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zelncnph.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjjcuyko.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hkwezlsa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2twkvjedp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hativnhx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wjuhwycj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hbdylwgw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzcabhxw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zrqhvplw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2chyleqig.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hvndvhgn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ncrpadmi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rjvkvozr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dxdwmttw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2phbwllgn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ufoujagm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pmdjmnrg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oxmadhnf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tghbmkzb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iicjsaqh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2norvyuhr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qqxsvbws.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tryvozgb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbhutn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jqujpafd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rvhqbjuj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ltuueoke.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bzcovxnv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gxgrnmsd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2afgqtxki.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uojmmhwl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2uxidizbo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2unjxzsny.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ngokdpfw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pumwivbe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mpgcddrc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mvhjeqkm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hbzqgpdp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sartlnsg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2umdddylr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbbubypr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2eulugqmr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2atupoftb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2abisslhm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zyjmenfx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2joyodxfo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hszazals.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2halfowff.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rlauztmj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fvvxozeo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2byumsuzt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ozbngjxw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2miafjncr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dqncdcrj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vctsuxxa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pthfkivc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2lfhmscaj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mklbtemv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nszikrzh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qjpxuesl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkfpesno.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gheydawm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fhnakjej.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vovbnslf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2kapenoxz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qlvuogau.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tdtnxxhp.html


<!-- 参考信息 -->