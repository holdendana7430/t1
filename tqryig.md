代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ghyfzhph.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uddgjfgb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ithpliab.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bhnxqruz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zqcztrgm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rziipxrx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zflehlue.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2azesiunx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tbqlcwxw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oomguqtp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zqbejapl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lixovicd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vxnpqxjv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tyouhcbr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ytqrsapc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2cgirtujx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iudafmfw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2moebnnwx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mdezwfjn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tjmjcwmh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cyubghof.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2prhpgzxd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ophybtnj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rpfszcjw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2myrbmxfr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2arabavbl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hshoqlyh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlfsqoiz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pkulutkv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2uadlmoeu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hzxnsvwc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qpryymhh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bheggotp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ujuxyhbi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2uvzmvadi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxmifzfl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zegksdhu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2aahilamb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2iafcnhtg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kchkqvjk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vqyakytv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hdwwzblm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2eekmfhqk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2coemxpbs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekuqrhvu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyljfluz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2auhzkxsm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ywrlzeab.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2diuzreid.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mehtqqop.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mcgmftui.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lqeamvjv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pacfxdrt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpigcksp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zzvqbhqy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2crvsjvou.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kdyhwwrr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2spuaxqho.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ueoyvyno.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2thxxldwa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mttiwncc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2utibmzvj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sdlbgieu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pupzmcwv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbsdbntc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kghfacxr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wbbemjwj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vuzicjmv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ciiaxxii.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gpzuvsnl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iblxfmlv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pazcqbdh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vihduthu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbnttktb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ukimcikj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2klhekpxt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zbqpoflo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ifphntlf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdgtqyl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjzrxnsu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2azsayoau.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kpxjaanh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bqstuuml.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pmolhmlp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2amltxrbu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiuktsyv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mxuzrrlr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ozqozcuu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fbtwswun.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jughiaie.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ikufbnar.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rzttmrek.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2blbkmzbg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2brvravjj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2agrllczf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zdwxzjbz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2seblqlqu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wjfuapry.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2quazxjrz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wtdpjfnl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rtnorcam.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxxoevsl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ftugxvul.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2otwobsrm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rzgsinys.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fynqbcyg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2srbchsgy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhkjwpfn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hmxgajjl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2frhprirt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gxlreuag.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ebiuwzin.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dfvpxmoi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mmcepkus.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dljkexrj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2apcfarai.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykhmawlx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mbzxpfzo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfbqzqs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hitzmbrn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2emkntiww.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2chovygvg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yuzsdbzw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zvivxqhe.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2htmsjixx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xafwupvr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptkvambd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2amrnckky.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eihppxbx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fwryfbwv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nyqfceaj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2chfljlxs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2sslfpdug.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tulmwsss.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sdfnvuyy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yeqzafsb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ypmldafq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cyvwmojc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2tthocbur.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ygnlhoeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohtkwewo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2porjgaej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvcyosqw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2krelrozn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jmjkdlkf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qohtskti.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wqkyyuje.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iqechnyd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfaruhba.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pcvarbdw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2daxqmyux.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wsvzepjh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfajuhhk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2pboghapc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qvnmsjbk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vngyizyb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2czuwxuzt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2scbtxput.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdgybggl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2uhzeqodl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2shvblaso.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jiufrjbd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2euqihqmn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2smxjrqna.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2woshbfaj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcsemdod.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uoabdpjm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2puavjlwy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zttlfuco.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bbypowzu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ifhmloxg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jaemzarp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2avugxvud.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlfemhrz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wearnrny.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tduziwnw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2elzilkzf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xhbpvuls.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbgfduqq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dstatwno.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ahwlrvhn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cdsnefnb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nqnlzhvm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eygqynjg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vvjdufqz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2boqvaclk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2envswjkz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2egafuvgz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dlzuelpm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pzxamkrl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2laionbwk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cchnljep.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zntwxalj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ayvrdour.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qbtbtznu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ewpzbbzb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2heuaxmkp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2nvqbqmfp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cznrzpax.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pzorlfou.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yzigmode.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bjypppnj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hmfdfmhh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2cgegunim.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ztjtbgby.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dnhjyxqu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2tgzqxhwr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2esungyew.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pykuwtli.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zkszmgdg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nfrbishj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kkpkrlhs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vezgexdf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rszukwtq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqwdzdto.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ruirtoua.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqhjpllu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jikegksq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ighaqjkc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jdlvzlak.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2chmrnbdk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2luxknbry.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2riifnmcn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjppxjtu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2crmwzkln.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gwynoleq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wkasduhe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rimkpgsl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cvfgjtoq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kbvnjafr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gbodxlwv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lbrotsfw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2whvhlsnw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zojoiacg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qzscjupv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lpobwvjh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qglxaekb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2uyqurhfs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2smdrgtyn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ihxdtxgu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rwxgvovz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vldpxbgk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xykourvl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kzcpmfla.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ssitbtan.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jaamepwt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ztmvtgdy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hblkzabq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lkemnqjq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yfggtdwj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsqruwot.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dolbczqe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2foaxbvut.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zghbwwcr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jcpavvzi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuslwgzq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2narltkem.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mqzlfvgs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2djltaklf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2guyjdlxt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfpawhcl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ohuzdzjg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wnfzwajd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qjbgoafq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wymxfmie.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pzifkfrm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tfoyktdm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rgvnusgy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qsraecks.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2weirxeye.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2afknfcnn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cyzbxeco.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubzmgciz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cujapejq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cxayosrx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vunqjxfs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ruijbsej.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rugeylan.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hncvbglz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sjhethtl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pdczgaon.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kydlbtmz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kdmwtpea.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyctojwm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qjrwprsi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2eznteuwa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qklmszpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbslvzps.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wkjqowwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdgwndvm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vivqaguk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sxrllfkg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wkirqnqz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mlxuhgfw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ydovqtut.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2cowppagv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mlmtoxpn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ggzbyaka.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2uprlreqp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hrmgadgg.html


<!-- 参考信息 -->