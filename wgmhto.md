代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2osrwdcxn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2whngyfqi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qkiykngi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jhljmpso.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ebhnensd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kvxpfizk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bflmqcxq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cbagzgxv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2sgybvcbr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vyosqiyv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2krwxunwz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fttosqfn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jsrijdvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quvrtwhk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jqcqktpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rodzhmcs.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mdgaegve.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ryrfnkce.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2knhqzigk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mywnxezn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2glucjgkb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wvozemln.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2aedshbfz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2oiffeooq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pwqpmuul.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qagnbdrl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xxedvrbi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lffdmtda.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zwbppczq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2umngclpm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nysjrxlu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2toxsqlsz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nbfffons.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2udcedlhb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dsfhclbb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hlpvpcpi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbrxdyhq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ifgopuph.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfdxdndi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbcidqfl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kqsmgyct.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xrgfnpxm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kaagxvdq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jeqqnvxh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrszgvs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzndqlag.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2akjwtltj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2crjwfacl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mkuloqmy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kybqsxcx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vxgluyoj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpyglqkh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2entzvkrs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2cppalnbk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ouwqlwdp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjkxjvaf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2whdfkhqj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgslekyk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcjzexm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fsabvrny.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2aowgsytw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ibgfylkb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mkcfofpf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xyauninh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2idmqimdr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bhxupppl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdwaccsv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rfjwqzwg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2asqctbjq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wewkuaeb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvibfsyu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbdbsrpx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mlncfhfi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qvanbxiu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vxchcdfe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuhkwuei.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2egxshbqx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ihnufloi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mhegpqhe.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hxudkapx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mqqrkpqh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fmdbpdhi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hwfzphlt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fflhsnvo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yjalvbwn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yqeyekoc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2joptytcy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ijqrquon.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2krayqlts.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gerdknfm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2djjtynhs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgntseio.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jljfflcc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lqjuqsti.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fhhbdqko.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gojxmjow.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2doxlwbtq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2csbecwjg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oabbwnlh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhceyoz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ugslfsxd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ehrmbioz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckgmddte.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vwdwsvnx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdjddcho.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xwagbcfq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hzvsmxsf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rqxgciat.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zqiqdwxw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dislwraf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2crhrdbtp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2sammisdm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dkahwrfn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mobuxsak.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2evuostmd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hvcoqxrx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uzklnodg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kzoyvebx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2patitzxy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zcvmcpjn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zootjyxs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2aumesujj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lyalrxdd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yastmsan.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dzwbjcyx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qtluwyup.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2aekevzim.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzzztns.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rggtbiyc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2invtfxly.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2heakfosp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2esgphqtm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxxypy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2aopsqluz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ufdvcuru.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2yvajrjps.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osovkdbp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecuqrdzj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hjftsoji.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xjfvabot.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzsoxjlm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2touwyqzf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2cenmabmr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bwzpkfzn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kezygoip.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2miziknye.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xhohtxas.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2judbspsg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nmcwqisk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxzizbel.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sbffraxe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2crdkokcc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tstnccfz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxyeoeq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2msxtzsrm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vchhedfl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fjwxknih.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ianejrho.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dmffvjuz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2oarkpnud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esdetppq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wsbjbypz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chpgyyqs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fexoaikl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2efexbnlx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtvpurhk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zmiutszh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xoucoduf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ojlevydj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sdscqooa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yunvflum.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cychcnum.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kxiykhoz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2stbsbmmr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2oxngxkac.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ylotwtzz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2riypeojc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gnfqxqcm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pyesjlhc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qvtlcjqt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rjxoznax.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcexffic.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nrnqoekv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2raxtqhpa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2shvvebmk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tndhxywv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzcmqgc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2llrstqug.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgwpyied.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xotynbjx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tfdqtrna.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ryzcodrs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fvqmschp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lyrsagas.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wjmamhqh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gbffgpvp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2bsxsstbu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lxmgwrvs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eyyhbkul.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qappjuwe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yygkpkjb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2dbawbcjh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gcdmllps.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2msauwtfl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zbnvmukv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rmsbyqga.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tnijlyfn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2udstcydz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jnjdnpgr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yoveunzz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uimoddrw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bwvpqinz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zpywvwtq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ahbjqtrq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qavbvarh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zsxxwnvy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gugrbopt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mqpikhis.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhordga.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rnfubvrf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pyxgmjgy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjhvmoa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gsrywmmb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fpvsfmyp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nblrejcv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ilooenxc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eyxvibsj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yzqrglvk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xziakoew.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yaqqfmjn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkxtoote.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ipyfkvwj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mbrvsmac.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2thwjukba.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mrpedoes.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrhlpwwq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2awmjbbeq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwiynky.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2juyftyoo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dgpighed.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtexilp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pqnunbpc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ysyvbllw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cshfbotg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yxvrxlyf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2byktbgcp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2neoyzbmy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2etcvgvwx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ondyjmhp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2whhxordn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wougucnv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jizzooci.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gaitbclg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zhrkbdzx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2piqluoex.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2omrannpr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2edjqgfmt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xmxjvcyp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zqsjtnok.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lpfrrflr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2khuevyiq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ztmlylgo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tgnmayod.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2siwrxrnh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hjskojct.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ciixgwjn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2icmgjchi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qejamkmw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jyysmpbp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mkoicbmz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2osudcjqe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qftebepe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2phbmcour.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imoenldh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2imuegryh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmmesuo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2juzbzkco.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cuqfehrt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hvoewjaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kjlfpouj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2drhptbsl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kinewqkx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yuqfovkv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ulbbiokj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2tnjltwzh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkykrqjc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mgmoadjn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cohmgczw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ortkkvwb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gpatwhqw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zwhtlmky.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2pqwcnazq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vbprytoq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btevvpxj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qfpqbsby.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jmzrluty.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ojfcdowz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ejqerpcg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rxwlwdnz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ulcbzsvo.html


<!-- 参考信息 -->