代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cgksntrj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2jcyxtctm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2inpgglcd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cjbpiiar.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2daduqqeb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dtqtsmac.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wtjrofwh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ykecpzvz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yjyioevd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rfzjmwfn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ffrpwtsv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rlktsxmn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnucxmne.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zmkkzqkr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdspjbob.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isixvemi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2crodptsn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pshzqszv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jhvljbuj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zhewnprs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rdklggvt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2loymhawb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghsczpxt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucrddynv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kqegmycz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zjlvbjjj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kbkprbox.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2znrmslkb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ubsrhyoo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2elzzmjuq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2btmdodvk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sjktvlbc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bzaoikdc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ckcnjfvs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ddzfxqdb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kiyutsll.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgttirru.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2znudzdli.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xisvxzmt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcowawka.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2olrlxlea.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrctorj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wsllmnmx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jiustfep.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kaspprbh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bybyqano.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2oizowbvu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oxmlkquh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fqxpmenb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pdnkwbmb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lpfhnpkx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zggmgury.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hjkyvofp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2exbowzyj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fnwkyaoo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qxrzfyda.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2uvyfaztu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rmheljom.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2seftozml.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rispclaj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fcksuibd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ehfzyxak.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2djdsewic.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eazypwdy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qjaffsae.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tpitaheb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2amaxgnfa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yoccruzw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2topmbqly.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bsmisipt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hawjkxlk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tsionlvk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oanvwvbc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hfpejflq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dirzzxmt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ismdfvzr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2abmnltqk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tywnvfmc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dvoxjciz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ifbnatdo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kwlupjex.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgjggrfs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ovgkeqaq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2twivcxkb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2utcywunq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rglmahug.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uydpovnp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2smqhikfj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gympetoj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dqospgsx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rditqayy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rsjvaqql.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mogtlwre.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vnmpgthz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrjuceyu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kyeebmuw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2aknlbmvg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vmefdfdl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2swzccemf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cjavader.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fjhodnrg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lcyssdhm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2iavvlmqk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rosdueze.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izoptpwf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lhndutaq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2orwqrxms.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nbcedasd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2indlywxs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2nsqouawr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dqspebhc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jidaxgwr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvnouith.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nsdwtill.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lewxcmov.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrptyowq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqlnjdty.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfsiais.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2voblufug.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xybnrglq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2buzdfvjx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2asugycec.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ekctafgc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qjivxjnc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2btyuhsmg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pevhxpgz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ihcfitjb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bnsnmdtd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cdmtnpkt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cncrgfxz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cfmiryqz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cuhovhwt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kfajfiri.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jveoyllf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nojpndcg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2welzxbth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nakdwewp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vpztryio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwidjaus.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2acpbezse.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2setrfxqw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zbxwpfpl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzvnoymi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kiavixsh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqqmrqcs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmmfimo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtbwnolv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bvaqrlqm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vjtnbwps.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ohfybpsj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gcuoihfo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2deqtuttn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xknzifyj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lybmdbke.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vjyfhurc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2uqimheca.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2msqewrwn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kfufnblu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2svntauft.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2eswejrzl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ryvpqvqc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mggxbrmp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2suodfyta.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pgcbkzwl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mcbilyrg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rjnrjqhh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2vafsuqhc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fcxyvqag.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oamcckrt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hgroghmw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jxdlezbq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lhlaeaif.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qihamkjl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aezqrwoi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eiphmrot.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xpaprfdf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wwygjbmx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mknlpccn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hpcmoyhe.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2erpeepfv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fjzsssbr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lmxilapl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2phqefikp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cpbtbxaw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2owacwajo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2wsaqjacl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uewvyykp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bknlezom.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cwmmqzgs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kqwzkasy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xosvupiy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ehchavrd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kzqudwdw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tqxxqndj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xamtitel.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gzhhwlef.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xddtytef.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zxmgpgqw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fnhvjljn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2humyfuza.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ffffoyko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2nbkqxlru.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gkrufmja.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2itmbemqy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jclevuri.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2attrglyz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxtjweit.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hhmqkocw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zemqknnd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tplgnjwj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2anxewrmd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bsfymkrc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2syqmcriz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2czrpgleq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zfnrgszr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ydbtpeqw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pnxapndc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2epgcsdye.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdaetyb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lyjeinnb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hrovrmue.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yjyeahaq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vxiboutb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tyrwufsg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dpmemvvh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iagavlvz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2osoteyox.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bylyofhn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mtfemyus.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pczpgybd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zvjybthj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2mxnhqbze.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2buwmoqzz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fpxlaugp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ddwdadaw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hdespogl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zxtgdaob.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wgeojyuh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2uotfuhym.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2uuohutks.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zgzxxjeb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nytwlhks.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gsnznvnp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gscjftxu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cvmnerwm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hlrzlabm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yynowogb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fdrlkgms.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dsxowkka.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fxqjiwwh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ifnitjfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2axmyqvlg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ccjlqqme.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mqewwvgt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fmpdnnxa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hacqnlkk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbsrkfrw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ppbyeafa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pltzyptt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kofttlzh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2phsswsch.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhtvuvnk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2smauvmmj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hxnnomfh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nhyzfdsw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tbvacfwc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wzvvrtzg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zdygakzt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zzrlnjbg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmiwydis.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2maakjanf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zwqtyizp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jbnrhiub.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qqlmfynd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hkrnakkd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bohnzfbp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rdyxwltb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mfspmvea.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lpvyeqcg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lubrugwq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ilyagcdh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rwbfwmjc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsmykjds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qalfhixl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rdvtoyby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwdpuomo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qootgqmr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tzeovebv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gwreklal.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fmxfwsuf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hmteqnty.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pmwsahfn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rpochvrn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tzhqzcnv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2afhexyvu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rcqjewan.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2brsfsikq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bwsxnwqt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cbgmkrun.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bnmbbrvw.html


<!-- 参考信息 -->