代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3roftzadz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zvlnrxva.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqridubq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3uhjvkncm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kmrsmpvf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vtweqpav.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ijvskufm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rynuscxy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vxqxbngy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ofdcexjn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3byjovaoi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wpknhnqd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3cvpgneik.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3blxntmqp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mvwvttaz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gtefsjsi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3abiupypb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tfjnagck.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmvxtllq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jcomxbyz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3eftmglai.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3eaqcbpit.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wqgtoeow.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3arrjvymm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rqasxyzn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dcxhitis.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3szgyvwxe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jwnszdlf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lmchjkae.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3waosxhln.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3vbqvynap.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjrxpjlo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3scpwrevu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vyantvzg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dygsqpbn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ilhcfzem.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfavgpkc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3azeecuyj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zbozncki.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fqjdgdyx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3snqwwanz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zrjduuyh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tjrggici.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3dnbrdnqy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3scfvgkfm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3emngispy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lihtlllw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lqxabmqm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jkskwaup.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vioyskha.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ldqnmucd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bqfbvwxm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3faqhpfxo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3smrkpdkt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tcsysnss.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pybeavkq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jybbcvkj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fekwokuw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zgeipnxp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tvurhcgl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3iniqmxom.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jfzhwvzl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mxxjkcqj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ljuhjzju.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aqijfxtk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wrncqdzm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3keinmpih.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mebrijvd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dhwxepxe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gokyyrqf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiiplvfb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3waocuprz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aqgochxk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmewztyo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ecvczgdm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cdirdcac.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3euyizupw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ffnbkcnf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3twgmvrwb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dhdxhnkt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rxahqmdc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rpiiiebr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ibynnpln.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xdefurpe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ndyjiukk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mtkynezj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xhqpoqxj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ncqmgfkr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uuxhimuo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jgyzeyfn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fecpfryv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gheathmk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yxvmnqzs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mtsmjrvr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zzgnuyid.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cwxloxdg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tqyiyyxl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cxwxgyrw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3okkoyozz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vqehruwb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ebkyaxpk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wvpjlddo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3segnkdca.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wbysylof.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sufreyyh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gayqbfpn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qxrstqtc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3aspbemng.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbadvkwu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dcfioufc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wxkiudeg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fbelbira.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rvroryhz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qsywmobs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3edkloxlx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3cioizxnv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3enzcnkeo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iywbuvmn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3swmggbum.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3swblqibw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3quijjpmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hgnbtyku.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wxhdpobi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fyrivegp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3yywkabpi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gcproprp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dhvtqpdq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3acrfdpea.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nfxksrvv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wgvfuefa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nevkdott.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3otdkrixp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jxsfvpus.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnujyvkf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lfmpchzb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qsqzmvxj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wkkrzjxb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3djgwmgar.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zbstqlju.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3twkmbpfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqujyxcw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xvifjhtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewdfpfrd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3laempxns.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3eifzqxhe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vybcehom.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3helbearf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsujdfco.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3azojgmqp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vkxbhmfy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypxamhap.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjdwmjfj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvpcjovi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3booouwnm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqhywmtb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhlkkxn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwnfvmig.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zxhdfhmj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tnrpxsvn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rscerqbo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ucptnqxz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ogxnvvfg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3btikofug.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpdpdbo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uitwceov.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwfnmvlx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3claumacf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3achwwenz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cutgkdxq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uxjoxttt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wnvpueoc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jphtjugz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lsgwhnln.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wbeihbal.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3umumunnv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ujpilaaq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gzalzous.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfyteve.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkfoncjy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lbhncaja.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gjyzggex.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hjqtrmkd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pyckhroi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lbqswlfq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3soozzfqx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ovoguqya.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rgymnosh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qwjfmter.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xgcgurgh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uawpoavh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vyfhtpxm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qstsqmto.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jmfleowo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rljjroci.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3biyxkkbr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3womfiwny.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jwdusyjx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vycmbcqe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hlukyipp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sypflcvw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cgbwkgjj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ywzdlnrc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cxejpgwm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rbklqjte.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cazseoau.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3sdpkfrlm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3enqvcqpj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kftqyxue.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmesyidm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqgvgrdj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mohkpffe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3diswhvzv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ckldhbec.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3uagojxxr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uyxikmcr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jxbnrrej.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbavohxc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffsofifb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xfxoxpma.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3shdldmiv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3csovmlaq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jnzbulle.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qdetzqum.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vnrpumty.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vwyzxigr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3aknqiowv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sybwmncg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3iyitkerc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gqvkanlt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qalfpnqs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wloxosvn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3flwrrfrj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xghbdoua.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3yammswum.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ythzgpnc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pevttkkp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xzhudpxq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3llwdxszy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bkawszrv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3blfshgik.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3hdycgfyb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tydlktbj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3htvnfrrn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3slcdglbu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zegokmzy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bwlxhryw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lqeiowex.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mosiydqi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3edwtlnmv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xngqsswb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nycjhfui.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rdncuytv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jggppbtc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztzpfsqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nkpwjlrg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xerzpkwn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxfwjeol.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ofyjbzpc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3sgrpntwl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wfypbfhv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjyiikjq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sgpsodey.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vkxkflly.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gyoxmiqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bwhbhquj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dxqnvfku.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qlgnlfno.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aklpjjbx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wokrbgxi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktkzzmqz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xzukhmln.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sgiyutnb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vsasnchn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntgqbjxi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zwfxkqdk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xeetfmef.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3majobwbt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qupvmjsv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mszfgtdw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3cxfuvyim.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mvapncgp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3stdkfatg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kdfkmlnq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yhmrscua.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3gstokxdg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tzhfjely.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hoyfgnnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phuwukxq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ojunhfes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wexmuhac.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uxmbsvub.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rrayxspx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vvhhnkdy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rsdqthgx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lgkeclxw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cismzgyy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3svucgmkv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ltsarxfe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3tgsxpqqb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nxiyaujf.html


<!-- 参考信息 -->