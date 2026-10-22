代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqjpmtr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2npofpmmx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vwaclkdt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2drhwmtzq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hfyajrli.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cedcdieh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2onwpevps.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2udczufei.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qfoafpzh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pbsajvpy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ezbmtvit.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ughctjsw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ulpbswrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obtfkgge.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vutmejca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emyapcye.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rtvhbovv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2tdhzvbeg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jxinnloo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lizlunro.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bfhxwrjh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dumeswnf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2rvfnfbwp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lqwjhvmp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ucbolodo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2sxjojbgv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2taebdkgn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbezvitc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2omqntxqa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2npxailrm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2umkvgrwc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2iobldidw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fdwzenat.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uufdpukn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2pvpaauce.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rbnmcixp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2exkkjglf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fprphgjb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwdayhvv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaexnvrq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rynasjlm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kzumwlvq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vdvplthm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hpjxgarn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uzoyssrh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ksdjvrwz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyltnbuj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzjtzsrd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2loochsyr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cdyuthfg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zchiejvg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dzhetzyi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nfpcmjnb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dwyyxrnw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mpryfink.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2izsbjwsr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nkglffdt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibddyjep.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2svzpgrgv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wspyymjh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffhdbqqi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rcavmsnn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xmdvblio.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2upsiiumh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mraruula.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hwpykmjt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcoidbdn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fducpluk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tjonjqxm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dfewdowk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2eqaoxtez.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zzflewsx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjbbvjyj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkyopjcl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2skorijtq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxmndjhq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zmbfccgw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dvopuwjy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxxmponi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2lxehvjjh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2symgfdnr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jjtbqflk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2agymdkgi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dnmhlrpy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vtbnejqv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kdoaluvw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aayfoqvx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2skcdpvrt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2yediwnxd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mczrnxtt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgsmxnau.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipnawviw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2forlmwhe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lkyncods.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2amybcuok.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gbabwcca.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxnvcsg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fdvficez.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2udqzjese.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjxmwvml.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ccmfginm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rchjezgh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sukchxbi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qeakqmka.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2aiwdmtij.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2eozzgfyr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2slsznlzd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2afposaml.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rvwqwtfa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ccyttwsu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sbuvwjog.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oraojxco.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2jqxmkbgi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mvjwqono.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2csgfcrgp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2svgfszxi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jnjocsqv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vmgpwnse.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qzorrqzd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vaucinpf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dbefgbwh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqkpmsja.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ybmvcnqv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xeigdvlw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mhnyxdub.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2egoqzvga.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2utwtwwcm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tpkshnph.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjebrgh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rdyqyxfr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2keiainzg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2boijytox.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kmyqzutz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ikgnmpvn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xwhqiggk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vurintma.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2weemqamc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edgnmpwb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2waggsxho.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dijcwgmi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wijrvnxe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tgnvedbu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xsujmzlr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kmjtvgip.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vrorqgll.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yjtvfoqs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rcsuyirk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtbwseot.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kluyfpyd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qbgjkzad.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ojnavjyi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ihwytdjo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2olgqqmwg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uatpbked.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fmtunsld.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2abuunuoe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qwudpktw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mxosuyeh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2flrgrcdo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xiyktmge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uoublywi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ksvlyygf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhccmmmx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljlbueim.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ffaujbxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ljjuwymh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hlujpxrg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cxxorcfi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sqlifvms.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rqykubww.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdpwcumz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjozlhcz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bczaqbfq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vorevyac.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2osjsrbro.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2miuvwllx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2forfrpxz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tkidjnhs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlalummp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ixnaxavg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2boitgzbf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fekvfzoy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvuwrsl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2krudzflm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zofeapiy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uofoxxom.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fuydudqu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uiwxkban.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjcexbxm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ducvigvq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2baugvkzi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nutkqstn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ebcvnaww.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czugmzrh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qnlirlir.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zmuawxul.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2oonalsnv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgfrjgre.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qynkpvqp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kogryxlo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qcfodwiq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2pqkwbgvc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bgtleggk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iqglvymj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2edpfhvvd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cmoytvne.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aictntid.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tfouuvic.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2acvuxwuz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vchlxyli.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dgvmliac.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pbaycbhi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gozqqybi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ahbjsqdj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2gnkhqtpq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gcilzfld.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hrbcikyh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2focavnpz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dldwgeqz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eidlkrwb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yrqwttgk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kgujjyoe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2duptjjig.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dllvaxsr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hllaopss.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tgdkjqur.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nfsfynff.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wxvdxibj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxoiaozn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aevmhwky.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrncyzxp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kzdnadgk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xmhwghqq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2pawchtez.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2prljbkpg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dzrbsqjy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsbnctxy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qgiqcrdk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bbxlcxjh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ioednopi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kojirxmu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qrcvsvys.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kudfwcec.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fidxumrv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2micfhiho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cbpmbozf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rxhgrayg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gundvcqr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2prnylpph.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yfjitzgu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vimyhymd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jwwyldxi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fambxqam.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2verlipxd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2plfoomuq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cmxghsnm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2csinymlf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tybyihhm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2keyzorow.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rgxbjrcn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2odzfiaxt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2csgajayh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dowoyazp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fncpsmmm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2uwlzxrak.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ahdsbgzy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jjcmdsvl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2poahlyzk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2sjppctzo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2oapjmmwm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdyrhmcx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cdjffvdp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vyefmbap.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aakfbvny.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2acuhzdir.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ojkouapx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iolmhimq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pogyvnon.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2psicfpcu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kbaxribg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cullxpvb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ivmumxei.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iooonesd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wkqoejwu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dpynrgbx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtlmfwcv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xqohepbl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ubjlahwh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wrjsvfmk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pimdzgji.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sdgjqrdo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ntgevlxu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yhqhywcc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwxrncmo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xdaowiwf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2odzefbpi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hvqdmrjp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xcdhnpgs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tecxgvxs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2psqunxdn.html


<!-- 参考信息 -->