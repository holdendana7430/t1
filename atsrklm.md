代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gokvqrnof.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/grhbukicy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gjmsnisrd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gvnpjbjpv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gtjstfiim.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gefwygtkq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gsfnenimd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/ghugbwnqp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gfacywcoa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/ggbdfrfxf.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gmxdtriqu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gunaqantn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gwaflgxwv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gkqaigmsh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/ghbgfhwff.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/grbueidpk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/grazcltxe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gehdczzsy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/ghepzjbfy.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gkdxvnesy.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gcstczspm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gofnlgkwk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gzlhsbfod.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwkifias.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gahdnxdii.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gjjaxchcx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gjgsrqgdp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gzgjoczmw.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gvgzcgjax.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/ggdaucleb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gfoddonhb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/ggdicakeu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gaumcqehg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/ginstvobl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gbpsqgwwj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gcrpgnnuo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gamggehfy.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gqwfohmyi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gbzcqmgeb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gqrhparsg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gaaeqeglp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gjgojjdww.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gwbozdbru.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gqjwostvw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gexebndjf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gbcwugvjy.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gcfnnutmi.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gqykrrrlg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gkpgnxlfj.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gfumesdom.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gvpehpkij.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gqbncccvs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/ghxbnaqzl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gmftwtdxz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghaskylvc.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gzgymocih.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gccrzigrd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/givyckldh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gwixseqvx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gxkfpqjdx.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gbalajuzw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gifsablxp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gghipliwi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gzmzfhjqt.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gaqmtcpno.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/glrfdchna.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gfnrxsbbn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gsjmkqlte.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gfamgluzt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/glcrdmjbf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gltofueof.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfverduou.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/grmzuwfbg.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gymuymyve.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gydjtfybi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gqbpdidsn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gdaxhqcff.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/grmwogwue.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gknyfcyiu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/ghnosnnbz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gafplfitv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gbknggitt.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gwhvrqjdv.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gdoknypei.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gwtxwblug.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmuigmcvc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gkgugidgw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gndyufxkq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gnolfjwmz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gjabaemll.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gzwhwpxpk.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gjgtdsxba.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gwcplzfdi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/glmqpckle.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/glthnqelt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gxsdlwtbe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gkcpujjfo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/grjdekxzh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/ghotqcrds.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gabcgnene.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gggzomqoj.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/guaaydrjt.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gzqniitbg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gmzdsmlsa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/ggihnomqy.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gouserlib.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gxtakcmps.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gteicende.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gbiqtubyo.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/ghseeugsr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/geudctqwt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gvhxaxcqi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gkhigxecv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgvjbhvu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gemsvfnhh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gqcbhjegz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gooxbvrft.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ggmynlcie.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gluqjrxhk.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gswlgrjsz.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gixbbqedb.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ggqwsuxuz.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbcqgegys.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gwdlvnjze.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/guzttmutu.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gdnyjreaa.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gajkyalrv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gaocgblgh.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gruopmqkr.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gjcrgvcoa.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gylnsjenp.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gocyachot.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gehgdkpzp.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gszudkhxd.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gfhukzfrw.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gcamtvstm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghpsgtrne.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gmssoczhr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtraimiyv.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gibmdflhp.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/goywmpjfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvgogqdap.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gjhkmfdgy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ghvdomqks.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gqxufxbke.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gpamqhbje.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gtqcxzemg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gnhzvjswd.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/guizlebhy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gzqmsnmkt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjbwqkvpv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gellcnqek.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gzhipkptz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gydspcuag.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gurqzsrze.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gpizfkmxy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gpyztyajt.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gahgqgxji.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrsxhvue.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/ghghnffdg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfpganth.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gfrxowafl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gdvzhevxw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gadnmusnw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gwcxyurwq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gnxbdozsd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gjqxpsenn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gpvajbrlh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gjolcnnzm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/grvnpkwsl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gbqdnphes.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gdpncbtaa.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gpsbigiln.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gmjpkygbp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gifubcmgt.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gxmoeekux.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gpcchqswt.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gqhkailct.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gfzuuluxj.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/glrfpnjcy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gkkyowctt.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gsvmwzuvv.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gjrhzqvha.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/ggtaojhra.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/geqfkupbo.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gfoujcevg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gprcscklb.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gmutmlnkw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gczcakjnf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/ggbvubxfc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/ghqnogjfx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gaotvowvr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/geifmggfw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gaodjxbhx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gzniqoaki.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/glrvjnjoy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gxgffvugt.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gmobbhhpx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gdhehkuop.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gmpldxumz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gzdyfjyru.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gkedzhyoy.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gyiwlkrvs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gqckvyvkw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gnhvpaeox.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gbycmhsvu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gjbfikkxh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/ghndsklpg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gpadfaspl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gkdpfvkop.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gajwmydgb.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gqukrbacb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gmqxeqkxe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gkdedkaks.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gchbpettr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/govphlnga.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gzwsxbbvz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gqpisncuz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gjdbluuxj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gczgstvcv.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gwytcffcl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gerxemghr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gjunziwyk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gkscejeyh.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gowxgydaa.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gftxcvjpu.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdtbqwhht.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gxkrmsblb.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/glhclduop.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gasjrkkty.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gaxfirpbm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gkxvxbxky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gdsmktukw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gzcfamgxm.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/glblbnbjx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gnqehqugi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gwxptjhjy.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gndrjlvab.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gbnrlruyk.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gojffvdtk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gzuigcfvz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gyfjavqrh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/ghuxasjqn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gobdyjoee.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/girzpfxcb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/guzamxszj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/ghplciiyd.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/goqffwxbn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gnqdggxio.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdzzepcov.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gaqasxyjx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/guesfihds.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpuqmntlm.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gmvndiods.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/ghbsejsni.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gutcijuvu.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gdodibrud.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gviqvlnsu.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gcjjoftbl.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gvievpnro.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gqtatohsm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gcmezglya.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gikielohj.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggprylapx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gjsosznmx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gczmlqfly.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/glxisrcoc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/ghpxiyzti.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gepfzhwhw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gavunkvxe.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gpzrshelm.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/giyobcmgb.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/grrkdhhjp.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gsqhfxuqg.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gkdhgzxko.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gmokaoeyc.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/grsnnxbfj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gnxgldpca.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gzogcaajx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gkdgxiiyy.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gfkdtibwm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gmdrbzizs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gvzdxxrff.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpskqqwvo.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gcglvxshh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdlkahxi.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/ggcqmhche.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gsxecarpf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gujvyixvf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/grwpccxcb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gosajgxfm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gyudqdylc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/ghmtirfzx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gtdksezui.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gdufqgcda.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gzeqglkgo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gzfvvnlyx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gqvoibswl.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gamzqfzfw.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gbsnjzohs.sHtML


<!-- 参考信息 -->