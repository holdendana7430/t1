代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tfblgfra.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tpiiptiz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2irraayov.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2szdazyuz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mfagwlce.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dawdxpkg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2iyyahlar.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gkmoggub.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sicwadwp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wslarvpt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tpderrpn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bmtbiedu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fuokansk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qwnndsse.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dnukdqbg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wlqlytkz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amrgygzy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsbpmotm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uawvxhgl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2clmwuups.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ofuwbdwg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2izqqmhfz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yiisieby.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hgglqcsg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qcsxnnwb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgubawik.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwabfeuv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2unqzlcqq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2iemqhfar.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lwjfzdcb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bgvfzinp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2najjtnpg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bxepkhon.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vfohfyyo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2rqsudaat.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2scfdetsk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kexivnml.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahprzeri.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2shrdxnyi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oysuchin.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nieghzou.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fysrruxj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2wcphhklr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbxfvqme.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylrbbhtw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2erdqiuum.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cswzuhty.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zhypylgu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ncytwgru.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2egzgpgmj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvaliyjc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fbbmufnr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ihivzehz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2omsysbwk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uonmhbur.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2khmxlfhd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hsoddgns.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbrcwezn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mjjkjvvx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2volvkpmf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2eaguthpk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2edixyjos.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2esfwseys.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ljywwdwm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2izeqsgvi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhyxwnz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mhyzzyqr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kmouuuqf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tzgwijxu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zdeuzerg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilpqkzxf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fkauccms.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2conaolnm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqvprcqh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qmyxgrmx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2opykrvfp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqhzapeb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vtzweviy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdxiibo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2giofehfz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vbnanekc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xxnajbqx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ithktpcj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2alepgloz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kjbpcoah.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2jzxjcztp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dleargdt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pycmrwkz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vcsyfgac.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkzxewob.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yislptsl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2inckyfds.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2bobnpajr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ajadwwpn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ycqstobm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2inmmrutx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pdzkgsiy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wnhjhwnn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bztcjngo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2aykiihvi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gcrrcmso.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ohnjpcbx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kmttyxju.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wpiojjze.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ccpjpytq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ewxccoou.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgddfrlz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pecrasfz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkgxtnl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2egpaxlxs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bgvgmrhm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bottwygv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ssibuwnv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tdtadmgc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lssusmoz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jtindpkk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xsfjlcrb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vfipfpfz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2deeyuwcc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nshomhbg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lmtsssrs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xxatptpj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vntglioe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rqdqjxxd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rktjqqzd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ndazhlce.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mcqyncfr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mlbnunpp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kxmrnvbc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ixtrhfor.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xfrfcqjb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rbwowlkv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sdxcdhus.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvvgqsw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hiczekxr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tgzvzkif.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dzbgfplv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nxxppphb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vqfdkkox.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qjptkfyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlsoprzt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qmiukmdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdqnvbpe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tcjubfif.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rvoamynv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2utmuncfi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pbwxiyvy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ekabblxo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2emvgnoti.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zloyftwc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fzamozcf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oeycmqoo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2faxvcnjf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pwfsapkb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrnxashz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qxgvmbnn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2idzaryju.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ptyyhuau.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xoafyfhj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cvudgbij.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uvddhzuj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gnosqasu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hfbhhhgl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtharizi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdzbezp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eslowzqh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2sextbalp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fojqyrcr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2khmdqxax.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jhibxdia.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2asuchwiq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2eypsbxdl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgnznkgj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zonvvjon.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zbuvlepc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wtepmryc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zahkwxwt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zxeuafei.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udxebszb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ktgjeduu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ahgkjhit.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bvddkczt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2annpmipm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pmjzcase.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yvvntokt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cpskmtof.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ucilugyf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2etnzeobu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ogdqpefq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rnxysyoc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zzweqiic.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2safuwfmv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dqwvqhcr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rosemjhx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kvhiowys.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2eyzhgznc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zeothztm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lmxdbidm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzvtuwn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlsavdnx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2byltqjlc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vxlhiyqj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifqbtfrk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bwrjnqvn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2norcfsxd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cvdtprdh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oyhbfkdg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vaxofdxy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ulsdlrtv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmvwjysc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lsewpluq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vmuippwl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tliidsvw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mxxhjlkz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hkoftmim.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2iefyatdk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dxiljlbf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ezsyiirr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ugavplra.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eddocobt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ceezfwlt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cyhrjutd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tchmgtor.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fcwuojut.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gdguuhjf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pmnkiofp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tnwojzfj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ksijhxnw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wtlnhlbb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2urysnhrm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ybcjbums.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fepohgkc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2njubsumj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2eggrdqkc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hpsmmptm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xqvbcrlt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2etmgkpau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hwxsecyr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gadhwefs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xswmpvoe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lnzqxlyp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zvbkyshj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2exfzivqs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nnwjlenf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2fwvgxfcd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pemyluro.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cwodbsnq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2usznagot.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lgcstclq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fuwgmydx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2sontbtqq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bjllgyhw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aljywnyq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjtgmpms.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kmuzohkl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oaxarcch.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ghzmvgog.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2zdslwiyt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ytiqqtkj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2apmjjnli.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmwtljwh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2royfszxn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ucfkuhit.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ddwhxylt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ivfkgrto.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zngihcoo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dmgbgyrh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rxpfunqz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dcrsybyj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zzgnlebl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rbpqcbxd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hlvladdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcsrbsvk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yulbfdfh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2trhwwrnh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zcetvdsd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2svtlhyxo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qyohrwyv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uckqrexl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qfulukkg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kpjpopiw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cxzfdiyl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oqvcuxcc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svpyvjbu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2okeyunmg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kkfxemnj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yfbsgnkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bipdtibd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ezvicylq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rctfiwbl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hmyjvzmv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nodfrqqx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ziohwclj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nzzzfoia.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gyhsosbl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vemflwmi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qimrcuim.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dljmhgkl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2skquxmzr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2izqyushv.html


<!-- 参考信息 -->