代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xbjhlylk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2amukktrc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yizbrvrz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bnyjhtxl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wbxjeojr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ljffqpfa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ijxaojpp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fswdndpc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2khzrmhdg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nuysscxe.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2umvqucap.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2evvueasd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vyepyxmc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zcbzwxux.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xyektqfp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftacjcnt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wuixothf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wexaejrh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2famklbet.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dxqfrunx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wngttmwc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwglknjs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qhkkmkex.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kwitxuaw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqtlxxqo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdbdabjn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kuypbqzx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2prirylyr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2prwwknce.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2iukvthzl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2eqibpkdk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oirpuppu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwhdiecq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2udxfpqzs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2glgzitpr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lvtudogt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2oxdindpx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2izymnpcx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ltryeorw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyvkyoia.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ysyypztz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sqvlqjvi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mnhqkftf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zzynrdbu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ulloffgi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2svplzzqy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2epvzrilj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2curpypnl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2stfiqxpo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmtlhmzw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hvzjsxkl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2llzcifnm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nzygadpi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fmbfbton.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2urooctau.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vvsepkqb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kmcortif.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bwuyefou.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wincdyzl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2thmnsibm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tjrcoxax.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2riiffbcz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2udfjtlmq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jfjjjxmp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2pidivzfx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hsmwgdud.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qmzvuijy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuxrazpm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwxggkzt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hlezlfoi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wezmpuvy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sojgwuze.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lqtnarez.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2knbhzwnl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cgougtml.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2kpvxqbco.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mfnfkrxs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xvnsabjc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvnedsof.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2foraobfs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hzyhzloa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2yxyxtcwe.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hrgvkepg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fvrkwepq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zsgmpewv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wivhukej.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mtobkltx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qsydqmns.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2snzebkbz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ihijwpim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ltwcozll.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jetoqofp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ovajspyr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zomisrtn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nniivikh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kknaiokx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tzjbjuzr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcxqoxas.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ohouqcxf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rzgfmoky.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2csqhfsha.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pnowemmc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnkyyida.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2endtciof.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rgsruclm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2riweszni.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wysqrdhb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wssnondu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vbjqbxwo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2decrethe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xelcjpyp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tfediarb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsffycib.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jyoewgas.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2znkyfugn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqyffsv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aplulqfg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2euphlwop.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2poypaapj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ujpqieoh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2exlrcxnh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hbndcnbk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hphxeqyk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sozydutm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mcaspzae.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2czyrujza.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zdbpnhgo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cstginuh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hsnbtddm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrdrsfrd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sbtvztsf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ryehhaic.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kxzpefle.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2grbxebnb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dzayrlmv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aztnexwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhyfcnwo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uuvylvbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owbajsuk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hwhyqfus.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jqfxkopm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2urxtwrwq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdicwdsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkjqowsj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2duejzwyw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dukddsss.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dgdqkyzv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdmobdmf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojzrzgdd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2uyjiikvf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtdwwjs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vctemury.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pisyyuqe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2wqjkethq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhtknzcw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jwcrgard.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rmpcnxgx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wetlgogq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pslserex.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2akvkmgts.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztnbzkdt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uvgifues.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2choojrcs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzucygu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijfppvrs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2oyutgnrt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2sbeexzwf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2swggxtej.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nkjlzkyb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfomfuzs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qkvywqpe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tdtekjfk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hknibeqt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rafisham.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbttjhqe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jjpyorxy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zbuvekjy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hrepbdpv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2scmewmhf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ukfzthht.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gguwxwvu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xjjcxnxr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jwrcujun.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nxoojmui.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xrsatsdt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2lynjptva.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mjflewtz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ihxagpwe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wfcokfzq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2imllfnyh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2acprpqyl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jwfcerok.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rqufyoqg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2klgduyno.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rfieifyn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ttpkfyqs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2roxwveii.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ljadmgvs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fvmgdcuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pthpzpab.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nawyskff.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dwngabxr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ljxqjati.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lwmtlqqq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziqvcgsb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mbnjmont.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukxpttyc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2biodoifw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2eyesdmxg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rhdsfija.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbhpbsgv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zdbazmxa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbyhsmuu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysdjdzym.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fchszrtq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2twrykyhm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2arrqvisn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mcusosna.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uneynvsz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2searmozo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2pmhmwztp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zgasuovi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2leegvknv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ngdwrkms.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2slupiucq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yksluozl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pkjmznye.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rxczqtcg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qvrnhhrt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wmshacyx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2okuynslk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vrmrttjn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xfedvevy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rfrwswex.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yngemstl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2csoeewmj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tzwawxeu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tdwklfnk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ijfhoatt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dlawjqlu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zufqmehi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ntzburds.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ygxvdzol.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fenaawju.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aajznlxn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uksxxolh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxetcobn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bbgkjcyn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vzneiuoh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbpswfue.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mdagswoq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbcowcfm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikcbtwgo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rogrpfny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2autawibc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tujvswao.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlyezbte.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ilchcuiu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2guzhqifa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nqcsxbdc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oosomuba.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbtjmwmw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dvjithhj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fnveagck.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xnpdmjiu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gtskkmpg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fvmrqthm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vcoqkoan.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ummzbuay.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wluaujst.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mrmmaqtj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bluiqzxv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qntbqtao.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dsnlckiz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2dbavmmgu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yfuotgmg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wmrwgccz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yhuvlktf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2akfcxzgo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qauiergc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jlvlrrfh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlygyuui.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xzbisytu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upyakord.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2duajchno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcirogps.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kayrrcqv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zhxpskuw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kbsjclpc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oaebeapw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vlxjyomo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dqgbzlwl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vruvuotk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tzjdqhks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nxlizhjg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xebeevdi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vcjsvesw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tvdprzrd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vkfisdfe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qoueruhc.html


<!-- 参考信息 -->