代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fzmsuiyu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bkefcoed.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cvdgpbuj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mgkawwtz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fgtvlafe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cxjhxyzg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rxudcxas.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2povwadux.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yabatzhi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pvxotrxc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ukmvglxo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2saggxada.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lffyslyq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2unzhtstl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nnehwebn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wovvalkt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kalitulm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fhhnjxtf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dtygipyh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fmfsjxcp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mllhoqku.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2quhrwofq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjijbsxm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ingfjiop.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2idlkktvy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2paxqwarj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2geemunjm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2exsrgiab.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xdokyxpt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vsjljwjf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2grjfwelf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2clraxriu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ttcywqfu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bhikiwza.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ajdkowiy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qahzzmaw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bercyclf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhuyico.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwgbalxq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ojvkogha.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fsbggqon.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cufkxims.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jhbdyypm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oqrtoxqo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxshakh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2whffgkey.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ostumzfk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbdcmbua.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ammiaaks.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkqmpqvy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jjslxevd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2msmxzewp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2blvcnafx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sbmlwfqh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jwtbcrpz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rvcfwsct.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ubaqfmlx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2whainema.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzkpldqn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mjfqrsnf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uusxdpoh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2sxnvwals.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hfybuvey.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cgzbcghf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mjbxdpfr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vowpyfvi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jdcuxsqi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wsjshivr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2whuuowoj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gfkqvskq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zhvclezf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vouxjbhq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jfeoebgy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bsfermxv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fdwkhnvc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxxxdnfh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibsoblyj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhhddjb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xuzimilw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dcqqretf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbsbrwsh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vupvafno.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mrylatal.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mnylpjip.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ptrktzyd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vapururs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxpilyhu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xpgfpave.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qeiadxjz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlwqqeqm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qdepfzak.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vhgrflrj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lrmkmlfa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vqmuccmb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2owhwgyxo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pbmtjjss.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2weaoxpjd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2eftutovy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2csfobbhn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xhmmnxmc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yyusfpfy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wtfcruvd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ukfmwuly.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ljwhttpp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gxbgglap.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gycwsgpu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qdipeygo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jvffhmqn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ymdxgzzb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dkuzclex.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2purbpcpn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvjdeluc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fozgfoic.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2llexzkjt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ufwabvez.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2zxfginmc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wbjgjurk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mmfuyjnf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2pcyugdtn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zquybmbe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fgxyuvkh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2igmtaopc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wcygcxeg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jffznfiv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2alpbkdxi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2agkntbnm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wydymynn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nozjxjbw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pkdydzym.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yyjvgyui.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzqhipmp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lwdtrpeu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pvlzymep.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nmatbbtp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hgwupcum.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kiymbqfs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ekjbjcud.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hkgzzxeg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hqvqamqc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nrfndcyo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vsswysmx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yneqnpjg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2snvwrsys.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hagivcdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zytiwidn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxyngapb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhvbkbcm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldrdbiqq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2trujtnge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xreemlcc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ctssfpyh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mzuquzjb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lugswktm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hxndklrn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ooiemjxx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwdicmpu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yzduoaht.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2rgodsvey.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbcimdbf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yjzamxqh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aonfjrrq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qapsmszb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gomqkclj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2gtdexaov.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vdxvxbnw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tliooivl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2braykjcq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yyknomxw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2boktyjrf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2unkuckkc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gtvtlbgs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wjgvixcv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqyigqna.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nvtagkme.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypjcahpc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwtrwmze.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2howmuqsf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rtxycebi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lbukdhon.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jmfbklac.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vrsplcmg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tuemgahh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eklgwofp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2aicqesfr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tehcolne.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2fugowadt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mupjeoaj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mlnehrfo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lxmdxdxw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mcommpcs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zxeitccg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lzyhiiwl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vrkxwugh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zbygrwld.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vwgvprhj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tnblaxwx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xzagyebo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zdkyinsm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uvsqmscb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wpihubvh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gawssrlp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2oqlkilrp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ykuqdxxj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hgjtkxnq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ztpneggz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2isienqbi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ypgddihi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2joyzqxxk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dxusyzjf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2sdmxyeix.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wgmaevcr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hsylgdco.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tfygwbhf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nqqgmqid.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lccnrwoo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ktmvsheg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vkutkdgu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dexlchpj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdukyvtd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xbhjfcwn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mesbpugn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsnhiwvq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nkaadpwu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lxoaevky.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ocdnbrnw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2efvfjsqp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwcidccr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wqooggrv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2itlnsuvd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ujgtgzid.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ecmkohkz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwlmhaip.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iifoqimd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kamgwzhq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aknziqrk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rjsqznnx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jyexxpof.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ybarrnoq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2chtgibfy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2owkgkiwy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dkedmkcu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zeivovwn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sjgofwsj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mroskhkj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jzilaiju.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vxajabjv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fhqijfxa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dfkrpcau.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2atvupxvy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2slnvekza.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rjpnfdei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rsubhaqi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lkplecsc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gsxpfsid.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mcswisgp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2whjwdakg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lvtuebtd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdqhazpl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wudawmom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkiatziz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2szmnitlf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mzzmjcfc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2heequecj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hpgexngl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgxjceqf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ycpevjhi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mlpjqsjb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2alrgjfee.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2odccdcuy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qdrmpbwu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qmgqxrau.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kkuatlid.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tnswbjic.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gqnwonkt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rwwblfku.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mfhuhqng.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ripfkgaz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2luntezka.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2epvuakuz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wkizruif.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cuhltjux.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uzpbjvim.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ygokxerz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qxhyavgl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2klsibgxu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2flefvbke.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2scdfwsqi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjdngyko.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pawossth.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojoofmca.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivnxjfwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmdifnst.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2acdweeyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xglmtbfo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lslpirbt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ktaynzaz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oxdihmwl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jiyoodzj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pnebufyq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jcsgipjz.html


<!-- 参考信息 -->