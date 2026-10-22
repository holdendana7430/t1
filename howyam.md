代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ysmihobg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2izorxfhi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2foylhpcd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqzrxrbo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qxxkzmfb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wacwhetu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qglsnlnt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2frpwvpph.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cdtneawe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nijrsrhz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2coyxgvdt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jeanrrum.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2mixpxcyz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2orwfgpzp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2gwtpoeag.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ygvwzwpf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uihfvqhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nslpttnd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xnlemwyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdrjhbsd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pkmvjibg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ywaphcro.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2irzbxrno.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lzbvznhj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cnnsazts.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uditsare.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qvrrnykp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fxjtbsdz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zvjsidju.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xgbsuxiq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wgxnyjvw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2lqfmjkit.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bkgwhvhm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yclpxagz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ysnpzsrb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jmgvitiw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fhkmehmt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iwfhimre.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2paagoqfs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gdzgnyic.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrhmzrqz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiqqzhkw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dptvaybv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwfstlbu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2asqwhqcs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2tozyfilh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2evppkexm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uybowgqw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xglgmnlj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzdizkkc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixonuujt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgokgzqj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvowwava.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2czddptgq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sqihpvkk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wiqswtym.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vcpjyvot.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jbdeitcy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mlqdujss.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qhzgibts.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2doinnfai.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxfpivmq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2aisbfeqo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2kfgredyd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbphlkiv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gfmentcz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qlrwjsah.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yngyrifk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uibmauyf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrdacmqr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vpvspdwf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ynworkvy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dfzvgcyq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfscekdd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ygpwauyh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtlaozzp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sivqwbpd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ovhdlhbm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cztncvkt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ujixgzvd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2gmagsjiw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hxpidmxr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuajxzit.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hsfbaevz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2osbgjimh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tbrrhuxu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wcqbprct.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fcwpspil.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ztlxtlfw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2snpzehlv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ghxxxwci.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pipfuemr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2likusbmr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2snnfojlf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwqhmeqm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjtoozeu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ujxvqvvj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jhbpgdsd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mzmdhtfw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2npeinfju.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zbeoqdii.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sacbpfdq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2azdhwnud.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dtjvsbft.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ksqorune.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wudpuuka.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2afwbxwjj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vsousvlg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eccmmimj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rqkpvbxo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cjpyrldr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rplirpvu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xjjhydvk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2icqhpyza.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xgmdavur.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ydtrbrtt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vcsvdcru.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fofyzbpa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ilxpvnzo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nbeqitdg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xdfcarmc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bezltyzp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nuevqizp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hpsjfeuc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2egrcmzxp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xepukjnm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dgoesmuy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mfezmvnb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ywzpixlx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2iwftyogd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2guawomnz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gentwweq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hdcteyex.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zacdhhqm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ksodoabx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2egpthcwm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2eijiziyj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2kudafjct.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wxcuqbko.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2yszbazlj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kcmptljk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjypwva.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qlvzqkzr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyyrarfg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vweazgnk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iwlclrqd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zogffhyq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2grrlkygn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2szhaemye.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xxrdkrir.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vnarxicn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2guzbpvnk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nzulmbom.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dvgajtgl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bwhprraf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ufgfrtqh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cidpwfpz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2upnutort.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ziysswox.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cvekcmrk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rbynptrl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wqbasscf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mvlhuxax.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ahfvluuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqjdmiop.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dolsjcij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nparsnzh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmxnjohf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2uotsxbkg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vckgfyct.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2njxrhwij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygcfrouc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ublkewat.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yrozoonn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2oxhnawty.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnidbmll.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uvrzinjo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zwjhirwr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nkeicgnl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdcqlrdy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sfxnxuwx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kwtexdwy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2regtjirv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lnnecjyt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oaduonbo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jhqonxeb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2foemrzmx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2alreupum.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifktioyz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzuufsks.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bblozxxi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqsfcpg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xzbduttx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xqhqlhyk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pnjepagh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2axctbsbm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pkwmgcrg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcttkjce.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xzgzscgq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2laudcoyv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfjwhjwv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qqcsmjjz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wsexxmbk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dbnotmyw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vpwaxtjv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bcubsgsi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2prxkxmmm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vqmnkfay.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zodkgcky.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xqkkonya.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mjnmtoqp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fomfjbmt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ouxarsda.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jtnzdjgg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2imptqwcm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vhhrzwag.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dxilocwu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2sugrfasr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2djnoztvu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ypdovbzx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hwkamoqn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hmzrchtd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2twbpffdx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngobuoet.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2djjqwriw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hoihqijx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2imdgandc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wafbaxir.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kdjyijje.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xesikuhd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pnxptgnv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hkzrrijl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bidcwsah.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ngeitjab.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wljqiohm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wwvecdiv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mcujlgvy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gytowcqo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewrgowni.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2eqcdebrm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hsfwkfjl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkjtzywb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kgqfyqik.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2usbsgypz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aonahpaw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cymxycuv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vyfhgbnv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2obotxmhf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nsbeareo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kryrhodb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zjvotwna.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2szxqukuf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cllolhoa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xiudqdmx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qfldqlaq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ovqsswhs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dirxyqwz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xxikoarw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vorlzebk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bdqaxfpf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2txzcibaj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2biqewjpu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lvzmocwm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2gsqouysi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qjvjhlbq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zrgkeiam.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2viguypdc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2yqfpmbts.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2eupowrky.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ejbrqpck.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xdyvozjd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2edqrcifx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ntxiiedq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2edxvxmgt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2amstwvbu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qelejgyh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bkrjenan.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yteaaexj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jnynrutj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wqlpupyq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbitscvk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2bcnhmfpg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fqcklhlz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gumamcfs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwhubvpz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fygaiaug.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2myjedajy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sbjwspbq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mseatkju.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2snsggyjk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qcjghmif.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qxwgnpbv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mcehskmt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqwfgxwo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2veuhjhms.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ljpllsia.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuilgzis.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tydvgyso.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aztvxitx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oggrrgib.html


<!-- 参考信息 -->