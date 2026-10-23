代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3duinbfvj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ggvryazh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kluwruhw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nnscpwvq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vrfkpudh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bbcoblbr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wzfggmeg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3snwpiewt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kqrxrvrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyqpvowe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wwjhejhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klldxiyf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xxsilrrz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gwgkiikr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3otckbrnb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nttrqimg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3prjnfcmv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3azfmxtlm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3euskueww.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ldbwyeyc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3acqlfzbz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3szpmewua.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vvfpdsqu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ienwvjzr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nzontomn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vvwqihfz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ggrjgoiv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vtznikna.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qfmyfnno.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qrnubgor.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pzwbjqlp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qdlirryb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mseeaebc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlxgztgi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulbrhptj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dzetrtzq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3etgmwhgy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wfxdbidt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hnsvuxrw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wcyycgnu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ldfqljkx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjzelrch.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppxssjla.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hpozqdwv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3skfwqkyn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3miwvntjt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zplqeqhk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxyfenma.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tzwsvjfn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uazhuywi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ofltifua.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmqwkvh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dhanspxk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnrrfifn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hwqkcswh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tbblziij.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3cjbhryru.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wiytuhyn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3inchyapn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpiebemy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yzzgfwxh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3otosgnny.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3trngykch.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rwuaqxwi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fzrrddck.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bwavmkho.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bkcllgfo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmaytz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xozhjcjn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3favqauzf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwcajovn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmijcxiz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3puualuxk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tduydrnn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymstgdbd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3wsjdzspn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cgewisdl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ibegfhar.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pvlarehl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xznwuouu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tcmtokqn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ytrjpaxy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ywdyxlic.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cxqrfube.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3duhjrikb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3liuosqxa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdanjfyq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3llxvfnci.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qigxyhcd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ivujkuzk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mghmadtg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ihtzcyiu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hsspfuae.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bhoholll.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ufktyebp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3luzauhwq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rbessqih.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jzfjoqzj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3psgdrbaa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxlirmws.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3axznndpm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfuycods.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3tbkolilt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3anqlnvmf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3krnhjueo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ykywzvmt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sluzcqnz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uinaspeb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vpoifinm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oxmdnyfj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkymhjml.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dijbhleb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jeujouib.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kkjkmjig.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3agyskekk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hgchaxxr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtznenqv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pjhyrmhf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cexyexba.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jagslokd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ysyjaiim.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3uuvogoth.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gadylzgo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ssrzzzqy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eocvrlpy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zkrbytxo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pdqjiydl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmfeuqw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dnssuimp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xdaasdqd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3amamkexw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vrahlpdq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdjpqkth.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gupzotfm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sosuhntx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpmolfqv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wxrxised.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvknozs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yiyejigc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hpwqfdhu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fhcvbckf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dwobpiix.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vvnwwrre.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nrgxtasd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nlkiqmkp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcjbwlvj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rgehbeeg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ignejvlh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pmfqyigm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3btrvmejr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3urlsumoj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jfoxdrwo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lczeceql.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3detvjmnt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3iedjvais.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vqxzqqqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffmttcan.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hbimxfyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrzuyrsp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gbiokiro.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bjhutpxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3thgqanzt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ovblfukh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3osxweaqb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ihhkwfei.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bpriqtrt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3msmokqyr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqpdmusf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gkvvdoey.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jrvvxyxk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hqiyyxvu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eahpzpfo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhefymqq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3esnttnxg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xafhgjzc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vrixdrdh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zjvxseim.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gqczuscz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3cstvxpku.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hnzepetv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pjczgepc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqqsrjxe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohlkzzqf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ahdktfhh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jbemeocg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3osnnokpn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3evbultey.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhxafce.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbjtizqg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zjkrxppi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xwdcewzn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uyltxyka.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lscmejml.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyeuwlrd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pfqjfuet.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wkfgqoty.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zgdisvug.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ioqaxhvs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ivisvqdf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ffsmoddw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pigvikvd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jkqintkw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3erqmzjpd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3judvvnil.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pvkfpuix.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3koqvddkx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3punyrjak.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pwchvumj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uekmcccx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fsrkxosu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gekyzkhz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uiggoqbs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eizopoey.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3patltjlf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3addcfsbg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zmdbiudl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dedsevur.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xczvifbl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kilfmrrm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jzkqhygi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkevftf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3yamznfsb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jastswof.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3sbfnbjtk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nwbgekbt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rlzamghl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yiuwjvnq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3uwjzxggz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3udzguukv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3fqdlvfug.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eavippar.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ixyycxnu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzerfehp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mskhsosc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3caiccwlp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cafdlsgi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3squsicox.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ebvboxkb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfaaiesq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rpqqgufi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3miitdkzl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tfneykzz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yppzvrof.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3evxhgdct.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yxwffifh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cmqezzht.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ukuanfbp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3twyruwwq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eewvltfn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ogkjanux.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3utlkxctx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kneevkqd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wjgvwlzx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uwvrvari.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dvzutjir.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ulajllxv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jtwqijpc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gstvwyie.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cihllkog.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bioqtalx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3aefvupwf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kzsbsigz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rafjflcw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rupaonfi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wtuxbhzj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fppuqztb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ioscntnn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wfpqcxen.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dundyhwn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3itrmscli.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zqoxfctk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbcrhdmv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jufjjqwt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rosubvib.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dqeckjjs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lfhxcqvx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpzxvhha.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jkjcvjae.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xtfrbieq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tasbmlai.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3saoarvsy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dqlmrywy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxnyxno.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lidcpakv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3tzthrzkw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xxjjlqwj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3iyagxpft.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lnwnkjkk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ozzusmxk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nczqpxbi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wqpdzdcw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oyyiyqoo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kxkkpcif.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3htifgwal.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dstbjlny.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rcndnujo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3uhgpmnix.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rzsficnj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kidxchsx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cffagkrm.html


<!-- 参考信息 -->