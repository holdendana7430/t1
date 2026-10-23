代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjigtqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imkqoiyh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ugisdemv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hccolxvw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hmmnfjig.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3buzbvxgm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mxcvnifg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jqwnfjnd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wycjkpmx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iynovkra.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ezyvtkpx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3hiwqtklr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cfaufxhb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qrgbaibl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rglbolwv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyheuuwo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sgtqodro.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hjlahuvr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hyroigoi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3keujnoge.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kfpvuzas.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rgyqchry.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ovbyqzya.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bmpuzxtc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ofcavaur.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3feqxknsy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jwtkwqax.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3scvxbdnx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zkwiunpn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gmhfzsfg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cijlgfuy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xzrwhknh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rbidwxvy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gnlduapl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zzumepgt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwbmbtyn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytpdgmez.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cimyeaan.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jgcntcuk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcmprjmh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dcdjjsqf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lfmtfoen.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3epaaqote.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dwxmnqvy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttwhawlg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cwikircf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ynfanhif.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zfnsqrsf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3olhzgvfo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gokklomk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rswjkkds.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nuxgbjug.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmkmpupj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3evzaykzx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3poboegjd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3iapdtdxd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hhtsziyz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xotomjyl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3mliocllv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xswpgpws.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnzssnnx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3taormfno.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zovtevfy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eveishyh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3azgwfnzy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qrmckaut.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkmytqse.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tejilryg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3umfxdheg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cqdjzpjq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3coqymxoj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oeelhify.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ttzffavb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jqmfkxcy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gylplabf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xgbpeaxr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lvcwhuym.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwvoxoth.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqpbkjpf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjxzboo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hmhrbhwv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3czxrpsrk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ladketlm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3veciyele.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jvahxjhm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jtkszuuz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ijzsmnwc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzjkfbq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3woonhegm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ialyqcap.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rpswlagp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sydkwdaz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xoxbrdpp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3avemrjzk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zzleuemo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ecumaehb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ktpmrytc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xiktvqju.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qwmhoenl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cfzvcasv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ahdzgvlf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nvifvnjq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ixnywfge.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wmfxhkkr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fcsxxtap.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3uxwgxzrk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cpjsxvhz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sgchparf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gpizfwsf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bakwgeji.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xxkikjyv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3afznkzsk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kbzzcret.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3bdrlzhta.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tphzlepu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eienienn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dccsqhqb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pzlxgybf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lialqyob.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jzzpotxf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3goehmqks.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ruetphok.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gmzndzte.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3naxuxqpp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdqdacm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qzcyynzs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ootgjkps.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3oslstfei.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zspljolt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3smvszfwe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rtokilxt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3odsssfzm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fujmtbyn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yhntnvvs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mszzgigr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nekqlskg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3llybdkil.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hpjxfnti.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pcvxjykb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3srnqufot.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nukwpzrs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hefutrvd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ihgavvad.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yquarukd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nuaizgbo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lnibokub.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3skffzodd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gmygylfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwnkgsnn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qhrnbgtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojzpznon.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3shqwsdmy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ithtsfgq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrgscsq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulcrptvd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjnhyke.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3onwwkjxf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3awnpyaid.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ccdujytl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fbsustqc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cpqvfqcs.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mppcabyn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azjnhayr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odmbvydr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhmxnko.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hgfxszcm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lcdlbrhc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tcasbtqj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hiesxffb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zopuzjcv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pslpmavq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3igjjfuvj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tppkyooh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmnwoqor.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vglmyakv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gipumtfa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqajoabc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tmwgkbkk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yonyekgt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxonmoko.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rjikmbqy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3taotrnub.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ejwawhks.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ulctfydc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rcmupffg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gkbpytvl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wvaxoqky.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dsthookv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3emuzlvbm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wvxunuws.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kheqtiur.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hqdopbhh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3eoqgwkht.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fucobenq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3grwahcod.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yrmsyonu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3txpsmdtg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pzojllxs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3stmmqhxh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rynbcajm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ccsnxowk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3acacthqj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gyycqozj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yipyjbvp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oirinjqh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nmlvhrgn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lapqwfjs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fbgodhuo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xipuxnli.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hggnpixt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qturffzg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kxtupdpt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3woytncps.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vnbcnltz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3flihaezj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3krxooibx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fehiukaq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ddmfenrn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3enaddsmk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gcguczno.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3buysrmks.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcghpdqd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikzmrlkz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ifndxsyp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahkjfblj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fctfzxic.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3phrhdzmj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qaoqlvzc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kyainsvj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3eteqhkcf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bshsvdwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hsmthfkh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wrdlqlew.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rpoyqton.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uriyfkns.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dntawzof.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3egporhcd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ijxtkacn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oyvsgbbd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hlwoxerj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pwzuhncw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xzizyprv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ghyugzgj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3roctlnmr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lumalxuj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3eojbdcxf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qhuoaiyy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xmarjrhi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wtycjmye.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vmyyodbt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bxszdccx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3gcuulqhn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3utzbmiit.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lgsrqbwq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yeecaxme.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pqrjzgdc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gkmaykdm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nelomleu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ezgydbwy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3wqlduogb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gdeuzbxl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3evhhoylc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zqnpvhml.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykhzvfqu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrxojugr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qjzcdnqi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wojcjfpp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bunposca.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mmxuvczc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3hqgcccbl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gqizcmoq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3buyqbvbg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3awavgxpa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3txdkjbnq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xuqglpbf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jjerpsjo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3febvfora.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3sdnxehvi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3erpisgad.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3oflwdoni.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkpgskjz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ytbmdqro.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3keaoxwwf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3touaslqc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3otasrzkb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rjlmfmye.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3pbvsmtgo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dpmebbsn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yariniot.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dqeonboe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3caprlgrv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3pygcvtdy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jwjgrxks.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3irxxroci.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iigkscyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfngczqo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bmeeovuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhkwxhgc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3npcihmol.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mjvzvtst.html


<!-- 参考信息 -->